## Untar multiple `.tar.gz` files to their respective directories


#### Goal:
This  

	dir/
		foo.tar.gz
		bar.tar.gz  
		baz.tar.gz  

Should become this

	dir/
		foo.tar.gz
		bar.tar.gz  
		baz.tar.gz  
		foo/
		bar/  
		baz/  

#### The code:

	actdir=`pwd`
	for files in *tar.gz ; do
	  filedir=`basename $files .tar.gz`
	  mkdir $filedir 
	  cd $filedir
	  tar -xzf ../$files
	  cd $actdir
	done

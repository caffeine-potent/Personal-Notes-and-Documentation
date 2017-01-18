# Configure
Configure doesn't configure your AWS account. It configures your connection to AWS.  

It asks for:  

- `Access key ID`: A short ID that someone in charge of your companies AWS account gives you
- `Secret Access key`: a longer ID that someone charge of your companies AWS account gives you
- `region`: Can be left blank
- `output format` Can be left blank

The code

	aws configure

List Buckets
=

	aws s3 ls s3://<bucket name>



Uploading(putting objects)
=  


The Copy Method:


	aws s3 cp my_file.tar.gz  s3://<bucket name>/my_file.tar.gz

- http://docs.aws.amazon.com/cli/latest/reference/s3/





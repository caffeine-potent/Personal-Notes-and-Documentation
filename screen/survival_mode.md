Screen
= 
----
	
###Create Screen


	screen


###Detach Screen 
- `Ctrl` + `A`
- `Ctrl`+`D`

###View All Screens

	screen -ls

###Attach Detached Screen

	screen -r <screen session #> 

IE.

> screen -r 12345

###Destroy Screen

Method 1:  

- Re-attach screen 
- type `Ctrl` + `A`then type `:quit`

Method 2:

- Type:  

		screen -X -S [session # you want to kill] quit
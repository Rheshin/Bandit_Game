Connect to the room
we have to find the open ports that are accepting ssl/tls transactions in localhost

nmap localhost -sV -p 31000-32000 
We have the following candidates:
	-31518
	-31790
	Other ports are echos :)
So we try each port to find the right one :
	- 31518 returns the same pass
	- 31790 is the correct one :)
Use the following flags : -no_tls1_3 (in order to use tls v1.2) and -quiet to have a smaller output(less verbose)

you'll get an ssh key to go to the next room :) 


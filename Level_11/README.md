Connect to the room
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
You have to switch each letter with its index in the alphabet + 13 (letter[i]=letter2[i+13])

You have to use tr : 
tr 'LIST1' 'LIST2' where :
	- 'LIST1' is the list that represents the inputs
	- 'LIST2' is the list that represents the outputs
In our case, we want to use the LIST2 as our alphabet where each letter is rotated 13 indexes later
so it will be something like '[N-Mn-m]', but tr hates cuts in the lists so we have to split it considering Z:
'LIST2'= '[N-ZA-Mn-za-m]'
the final command is : 
cat data.txt | tr '[A-Za-z]' '[N-ZA-Mn-za-m]'

get the passwd and see you in the next room :3

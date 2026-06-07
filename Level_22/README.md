There's a cronjob that executes a bash file in /usr/bin/cronjob_bandit23.sh
We can see that it copies the passwd of the bandit23 user into a file that is in tmp
and we can get the name of the file by repeating the cmd that generates its name 
"echo  I am ... | md5sum | cut -d ' ' -f 1"
and then when we read the content of this file, we get the passwd for the next room


Connect to the room 9

"The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters."

We have to filter the file first, using strings.
Then we can just grep the password using grep "="

(strings data.txt | grep "=")


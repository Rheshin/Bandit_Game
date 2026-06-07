Connect to the room 8 
We are seeking for the unique line inside a big chunk of data

Cat the file, pipe the result with sort to get the duplicates near each other, then use uniq -u to delete all the lines that are duplicated :) 

( cat data.txt | sort | uniq -u)

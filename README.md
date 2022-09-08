# WordCounterCLI
Unique word counter for a text file using Linux CLI tools
 
## CLI tools used
	1.  cat othello | tr -sc 'A-Za-z' '\012' | sort | uniq -c > newfile
	- This reads in the text file "othello" with cat. 
	- The tr squeezes the characters from the standard input and replaces then with a single occurence. 
	- Sort simply sorts the output
	- uniq -c counts the occurances 
	- > newfile records the results in a newly created text file "newfile"
	
	2. tr -sc 'A-Za-z' '\012' < othello | sort | uniq -c
	- This version has the same effect except instead of writing the results to a text file, they are printed within the terminal.
	- example output:       
	452 a
	72 A
	1 Abandon
	2 abhor
	1 Abhor
	1 abide
	2 abilities
	1 ability


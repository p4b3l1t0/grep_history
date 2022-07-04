# Grep the history of commands executed

This is a manual to install a function in your shell (bashrc or zshrc).

###You must add the following function to your shell terminal:

	h() { history | grep "$1" | grep "$2" | grep "$3" | head -10 | sed 's/[^ ]*  //'; }
	
###Save the file and execute:

	Source ~/.bashrc or source ~/.zshrc 
	
###To use the command you can execute:

	h "command to search" > example: h ls


# Grep the history of commands executed

This is a manual to install a function in your shell (bashrc or zshrc).


	1 - You must add the following function to your shell terminal:
h() { history | grep "$1" | grep "$2" | grep "$3" | head -10 | sed 's/[^ ]*  //'; }
	
	2- Save the file and execute:
**source ~/.bashrc or source ~/.zshrc** 
 
	3- To use the command you can execute:
**h "command to search" > example: h ls**

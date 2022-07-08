# Grep the history of commands executed

This is a manual to install a function in your shell (bashrc or zshrc).

###You must add the following function to your shell terminal:
#### for ~/.bashrc

	echo "h() { history | grep "$1" | grep "$2" | grep "$3" | head -10 | sed 's/[^ ]*  //'; }" >> ~/.bashrc
	
###You must add the following function to your shell terminal:
#### for ~/.zshrc

	echo "h() { history | grep "$1" | grep "$2" | grep "$3" | head -10 | sed 's/[^ ]*  //'; }" >> ~/.zshrc
	
	
###To use the command you can execute:

	h "command to search" > example: h ls


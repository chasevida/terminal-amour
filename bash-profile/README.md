# Bash Profile
A `.bash_profile` file lives in your home directory and is called everytime before the Terminal is launched. It allows you to set up custom environment variables such as path links and shortcuts as well as a slew of other cool things.

The `.bash_profile` is a system file (hence it starts with a `.`) so it's hidden from view in a traiditional Finder set up. You can see if it exists by opening your terminal and typing the following commands.

	$ cd ~/
	$ ls -lah
	
You should see it displayed in the list, if it's not there then you can create it using the following command.

	$ touch .bash_profile
	
To open the file in a simple text editor run the following command.

	$ open -a TextEdit .bash_profile
	
You should now be able to view all of your default configuration.

## Paths
You will most likely already have a `.bash_profile` with some paths set up. Some helpful paths to have if not already are the following which should be placed near the top of the file.

	PATH=$PATH:/usr/local/bin
	PATH=$PATH:/usr/local/git/bin
	
If you're using php alot you may find these helpful to have with [composer](http://getcomposer.org/) installed (preferrably globally).	

	PATH=$PATH:./vendor/bin
	PATH=$PATH:~/.composer/vendor/bin

## Git Branching Fun
We can customise the terminal to output the name of the git branch and it's state if we are in a git repository. To do that we can append the code found in the [git-profile](git-profile.txt) file to our `.bash_profile`. It's best to add this to the end.

What we will get with this should look like the following when inside a git repo.

	project-name [master] $
	
When we have uncommited and unstaged changes the `[master]` will display red to let us know it's state. It will be blue when changes are staged and green when everything is commited.

## Git Aliases
It's helpful to have some shortcuts for common commands to save time. Below are a list of some commands I've set up aliases for, you might want to add your own, the format is pretty straight forward.

These are listed with all my aliases in the following [aliases](aliases.txt) file.

	##############################
	## Git Alias
	##############################
	alias glp='git lg'
	alias gs='git status'
	alias ga='git add'
	alias gau='git add -u .'
	alias gcm='git commit -m '
	alias gpa='git push --all'
	alias gpm='git push -u origin master'
	alias gpd='git push -u origin develop'
	
	
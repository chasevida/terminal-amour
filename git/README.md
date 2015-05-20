# Git
As you know git is simply awesome and incredibly powerful. There are also some great extensions that make it even more so.

## Plugins
Check out this great package that adds a whole lot of extras to git.

* [Git Extras](https://github.com/tj/git-extras)

## A better git log
The git log is great and all but some people have taken it [upon themselves](https://coderwall.com/p/euwpig/a-better-git-log) to really make it beautiful.

In short you can type the following command into your terminal to create a nice shortcut.

	$ git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit
	
Now when you type `$ git log` you will see your log output something beautiful.

## Default Editor
While we're at it perhaps we may want to change our default git editor to vim? To do that we can do the following (ensuring we have vim installed obviously).

	$ git config --global core.editor "vim"
	
## Global Ignores
You don't want to have to commit a gitignore file that includes system specific ignores. To get around this we can have a global git ingore file. This should live in your home directory.

	$ cd ~/
	$ touch .gitignore_global
	$ open -a TextEdit .gitignore_global
	
If it exists great, otherwise we can open it up and start adding things like `.DS_Store` etc.
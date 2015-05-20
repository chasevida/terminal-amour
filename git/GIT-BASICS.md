# Git Basics
A real simple overview of some basic git commands that can be used from the terminal.

	$ git init                    // creates a new repo
	$ git --help                  // list help instructions
	$ git add .                   // stage all unstaged files
	$ git add -u .                // stage all files including those deleted
	$ git commit -m "message"     // commit staged files with message
	$ git log                     // show the commit log
	$ git log --online            // show all commits condensed
	
## Branching

	$ git branch                             // list all branches
	$ git branch myfeature                   // create a new branch
	$ git checkout myfeature                 // switch branch
	$ git checkout -b myfeature              // create branch and check it out
	$ git merge myfeature                    // merge branch
	$ git merge --no-ff myfeature            // merge and create a new commit
	$ git branch -d myfeature                // delete branch
	
## Remotes

	$ git remote -v                          // list remote connection
	$ git remote add origin [url]            // add a remote repo
	$ git remote remove [destination]        // remove link to remote repo
	$ git push -u origin master              // push local repo to remote repo
	$ git checkout --track origin/myfeature  // track remote branch
	
## Tags

	$ git tag -a v0.1.0 -m "message"         // create a tag
	$ git tag -a v0.1.0 -m "message" 8cbg3s  // create commit specific tag
	$ git tag                                // list all tags
	$ git show v0.1.0                        // display tagged commit
	$ git push origin [tagname]              // push a specific tag
	$ git push --tags                        // push all tags
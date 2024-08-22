## Git Cheat Sheet and Branching Practice

Examples of common git commands. Also practice dealing with branching anfd resolving merge conflicts.

Stuff added in main branch.
More main stuff.

### General Commands
* 'git init' - initialize local git repo in current working directory
* 'git add filename' - stage 'filename' for commit
* 'git commit -m msg' - commit statged files into local repo

### Information Commands
* 'git status' - show of local repo
* 'git log' - list commit history of current branch
* 'git log --oneline' - list commit history (compact format)

### Remote Commands
* 'git remote add origin url' - add new remote 'url' with alias 'origin
* 'git push origin branchName' - push current local branch to remote branch 'branchName' 
* 'git pull origin branchName' - pull and merge remote branch 'branchName' with current local branch

## Workflow:
1. Pull latest remote main into local main
	```
	git pull origin main
	```

1. Branch from updated local main
	```
	git checkout -b myBranch
	```
1. Work in local branch, commiting frequently
1. When ready to merge, pull remote 'main' into local branch (must commit first)
	```
	git pull origin main
	```

	* Fix any merge conflicts, then commit
1. Push to remote branch
	```
	git push origin myBranch
	```
1. Create pull request
1. Merge Pull request




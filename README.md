# Git Tips

> Git Tips to work.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT9oB6jmPaiNkrASSSnNGoJPAs4CRLtRFA7pQ&usqp=CAU)


> This cheat sheet features the most important and commonly
used Git commands for easy reference.


# 1. Create a new repository on the command line 

Get started by creating a new file or uploading an existing file:

	echo "# gittips" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git branch -M master
	git remote add origin https://github.com/peteralexandercharles/gittips.git
	git push -u origin master
    
    
    
# 2. How to list branches in Git?

The command to list all branches in local and remote repositories is:


	$ git branch -a
    
# 3. Create a new branch based
Create a new brach based on your current HEAD

	git branch <new-branch>
    

# 4. Merge

![](https://miro.medium.com/max/1204/1*cEXnJtDL2tGeoN3KoCJSIw.png)

Merge <branch> into your current HEAD
	
  	git merge <new-feature-branch>
  

# 5. How to delete a Git brach locally and remotely

Git will not let you delete the branch you are currently on so you must make sure to switch to branch that you are NOT deleting. For example: git switch master

Delete branch locally:

	git branch -d localBranchName
    
Delete branch remotely

	git push origin --delete remoteBranchName
  
  
  
Sorces:  
[An introduction to Git merge and rebase: what they are, and how to use them
](https://www.freecodecamp.org/news/an-introduction-to-git-merge-and-rebase-what-they-are-and-how-to-use-them-131b863785f/)
  
[How to list branches in Git?](https://www.jquery-az.com/list-branches-git/)
  
[How to Delete a Git Branch Both Locally and Remotely](https://www.freecodecamp.org/news/how-to-delete-a-git-branch-both-locally-and-remotely/)
  
  

  
 # Back to the previous branch
  	git checkout - 
 
 # Cherry-pick but with autocommit
	git cherry-pick a6817b7 sdfasdf
  	# .... as many as you want
  
 # Cherry-pick without commit !
  	git cherry-pick a6817b7 sdfasdf -n
  
# Time Machine Back to Past and Delete the Future.
  	git checkout <commit>
  	git push -f origin <name-of-remote-branch>

  
  ![](https://emojipedia-us.s3.amazonaws.com/content/2020/04/05/yt.png) [Youtube - Git cherry pick tutorial. How to use git cherry-pick.
](  https://www.youtube.com/watch?v=wIY824wWpu4)

  
  # Undoing the Last Commit
However, of course, there a tons of situations where you really want to undo that last commit. E.g. because you'd like to restructure it extensively - or even discard it altogether!

In these cases, the "reset" command is your best friend:
  
  	$ git reset --soft HEAD~1
  
  Reset will rewind your current HEAD branch to the specified revision. In our example above, we'd like to return to the one before the current revision - effectively making our last commit undone.

Note the --soft flag: this makes sure that the changes in undone revisions are preserved. After running the command, you'll find the changes as uncommitted local modifications in your working copy.

If you don't want to keep these changes, simply use the --hard flag. Be sure to only do this when you're sure you don't need these changes anymore.
  	
  	$ git reset --hard HEAD~1
  
  # Undoing Multiple Commits
The same technique allows you to return to any previous revision:

		$ git reset --hard 0ad5a7a6
  
Always keep in mind, however, that using the reset command undoes all commits that came after the one you returned to:

  ![](https://www.git-tower.com/learn/git/faq/undo-last-commit/02-reset-concept.png)
  
 # peteralexandercharles/git
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT9oB6jmPaiNkrASSSnNGoJPAs4CRLtRFA7pQ&usqp=CAU)
   [GitHub](https://github.com/peteralexandercharles)
   
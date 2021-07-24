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

  
 # peteralexandercharles/git
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT9oB6jmPaiNkrASSSnNGoJPAs4CRLtRFA7pQ&usqp=CAU)
   [GitHub](https://github.com/peteralexandercharles)
  

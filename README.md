# HW1-WE-Question-3
 A Repository for Web Programming Course Homework 1 - Question 3

**Part 1**

you can add your *staged* changes to your *last* commit with *"git commit --amend"* and you can use *"-m 'new comment'"* to change the commit's comment

**Part 2**

this command, deletes the my.env file from the cache of all of the branches: 
*git filter-branch -f \
 --index-filter "git rm --cached -rf --ignore-unmatch my.env" \
 --tag-name-filter cat -- HEAD*
 then with *git push -f* you can force the changes aginst you repository. 
 
 **Part 3**
 
 you can add your teammates repository to you own using *"git remote"* command. each user has it's own local repo and can access the main repository via *"origin"* which is the name given to the main remote repository. *remote repositories* can be added to you local project and will be saved in ".git/config" file with their URL. so you can access your teammate local repo by adding their local repo as a remote repo of your own. you can perform *git pull, git push and git fetch* against every single one of the remote repositories if you are granted the access.
 
 Another way to accomplish the scenario requested in the question is by using *"git branches"* which is something I have done in this repository. In this scenario I create a new brnach for me and my teammate on remote origin which is the main repository and push the commits to that brach. my friend can access and change them and merge them to the master branch of the original remote repository whenever they want. 
 
 
 **Part 4** 
 
 picking specific commit from another branch can be done by  *"git cherry-pick"* command.
 inorder for making multiple commits into one single commit before merging them, you can use *"git rebase -i HEAD~n"* to view n last logs of your repository history and then *"squash"* all n-1 commits into the first commit among them. *sqush* makes a single commit out of n commits. then you can push and merge the squshed commit. 
 
 

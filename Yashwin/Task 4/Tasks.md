# Task 1:
## 1.   What do you mean by git and GitHub?
Git is a Distributed Version Control System. Git is an open-source software which helps to maintain a different version of our code and track all files, by providing many different operations. It saves us from server failures by creating local copies of our code. It lets us work in offline mode too.
GitHub is a web service where we can have projects that have version control over them.
 
## 2.   Why GitHub is so popular and used in most of the projects?
It provides Git features in an easy-to-use way so that even a beginner can perform Git operations without having to know about programming.
It provides Cloud Storage.
 
## 3.   What is a version control system? How Git is a VCS?
Version Control System is a software that lets us maintain a different version of our code and files.
With this, we can change the version of our code at any point, which means we can go back to an older code with just a few steps.
Git provides the above-mentioned features, which makes it a VCS.

## 4.   What are the other platforms similar to GitHub?
BitBucket
GitLab

## 5.   Why are you interested in learning of Git and GitHub?
I work on android app development, where git is very important.
Also, I want to work more on open source projects and git is a must if I want to go in that direction.


/////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

# Task 2:
[GitHub repo](https://github.com/yashwin1/github_series)

## a. How git workflow works?
First, we create a repo or fork or clone some other repo
Then we work on that repo, i.e., we work on the files present in our working directory
On adding a new file to our working directory, we use the git add command, which places the new files in the staging area, which is a step in between the working directory and the local repo.
In order to add the new files and any changes that we have made to the already added files, to our local repo, we use the git commit command.
Finally, in order to add/update files from our local repo to the remote repo, we use the git push command.
Now, in order to get files from the remote repo to our local repo, we use the git fetch command, and to get the files to our working directory, we use the git merge command.
This lets us see the differences between files that are present in the working directory and the ones that have been fetched from the remote repo to our local repo, using the git diff command.
We can directly get the files from the remote repo to the working directory, using the git pull command.

## b. What're the different stages of a git project as commit, add?
On adding a new file to our working directory, we use the git add command, which places the new files in the staging area, which is a step in between the working directory and the local repo.
In order to add the new files and any changes that we have made to the already added files, to our local repo, we use the git commit command.
 
## c. Is it possible to do a git commit before git add if you have made any changes? Explain why?
There are two scenarios while making a git commit.
The first case is, if we have added some new files to the working directory. In this case, we need to do git add first, to add the files to the staging area, and then a git commit to add the new files from the staging area and the changes made (if any) to these new files as well as old files, to the local repo.
All the new files do not go to the local repo from the working directory directly with a git commit. They need to first pass through the intermediate state, which is the staging area via the git add command.
The second case is if no new files have been added to the working directory. In this case, there are no files to be sent to the staging area, so there is no need for a git add. We can directly do a git commit.

## d. Why is git diff used?
It is used to get the differences between the current status of the project (working directory) and the local repository.
It shows the lines that were added and deleted, for each file in the project.

## e. Can we leave the commit message as blank?
By default, git does not allow to leave the commit message as blank because providing a meaningful commit message is part of good development practice.
However, newer versions of git have a command-line argument, "--allow-empty-message" which lets us leave the commit message as blank. The command then looks like: " git commit -a --allow-empty-message -m ''" "


//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////


# Task 3:
## 1. Share the link of the PR you have made, so you need to submit the link of two PR's.
[PR 1](https://github.com/codewayy/github_series/pull/202)
[PR 2](https://github.com/codewayy/github_series/pull/203)
 
# Drop the answer to the following questions
## a. What is meant by the term fork and clone?
To contribute to someone else’s project or to use someone’s project as the starting point for your own. This process is known as forking.
Creating a “fork” is producing a personal copy of someone else’s project. Forks act as a sort of bridge between the original repository and your personal copy.
Forking makes a copy of a repo on GitHub, but in order to work on the project, we need to get it on our computer.
This process is called cloning. Making a clone of the project to work on our own computer.

## b. What are branches in GitHub?
A branch is used for creating a side track from the main code (or from some other branch) to work on some experimental code which we are yet sure about and would want to stay separate from the master branch or the main code.
 
## c. What is PR?
After cloning a repo or creating a new branches for a repo, we make changes to the new branch.
After making changes to the new branch, we need to add the changes to the original repo or to some other branch.
This is done by making a pull request(PR).
It creates a request to add the changes made in the new branch to the original repo.
A message is associated with a PR to provide information about the changes made.
 
## d. Can we delete the master branch if not. Why?
We cannot delete the master branch since it is the default branch of a repo.
But, if we move the HEAD or default to another branch, then we can delete the master branch.
 
## e. How can we delete a branch? (Explore a bit about this yourself)
There are different ways to delete a branch which depend on the state of the branch.
Command: "git branch -d <branch name>". This command is used to delete a branch locally when the branch has already been pushed and merged with the remote branch.
Command: "git branch -D <branch name>". This command is used to force delete a branch locally even if the branch has not been pushed or merged with the remote branch yet.
Command: "git push <remote> -delete <branch name>". This command is used to delete a branch remotely

Task Day_1:-
1. Git is a distributed version control tool that can manage a development project's source code history. It is a tool a developer installs locally on their computer.
On the other hand GitHub is an online service to which developers who use Git can connect and upload or download resources. It is a cloud based platform built around the Git tool which stores code pushed to it from computers running the Git tool. 

2.Git is widely used because it provides cloud storage for source code, supports all popular programming languages, and streamlines the iteration process. It's platform controls revisions and runs in the command line interface. It is an Open-source platform.

3.Version control systems help a software team manage changes to source code over time. VCS keeps track of every modification to the code in a database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake.
Git is a distributed VCS, where every contributor has a local copy or “clone” of the main repository i.e. everyone maintains a local repository of their own which contains all the files and metadata present in the main repository.

4.Other platforms similar to Github
 -Bitbucket
 -Source Forge
 -Gitbucket
 -Beanstalk

5. Features such as open-source, availability to use various programming languages, able to clone files, edit code,etc make me interested to use Git and GitHub.

**********************************************************************************************************************************************************************
**********************************************************************************************************************************************************************
Task Day_2:-
Q1. How git workflow works?
 ans:- Git Workflow consists of 4 fundamentals.
1. Workspace - it is the local directory 
2. Index- it is also called as stage
3. Local Repository- Head
4. Remote Repository
If the file is in workspace,it can be considered in 3 stages:-
 committed, modified and staged where the file can be safe in local repository, locally modified and a file can be updated in next commit respectively.

Q2.What are the different stages of a git project as commit ,add?
 ans:- Files in a repository go through three stages before being under version control with git:

Untracked: the file exists, but is not part of git's version control
Staged: the file has been added to git's version control but changes have not been committed
Committed: the change has been committed.

Q3. Is it possible to do a git commit before git add,  if you made any changes. Explain why?
 ans:-
No, A file won't be automatically included in the next commit just because it was changed. Instead, you need to use the "git add" command to mark the desired changes for inclusion.
Using the "git commit" command only saves a new commit object in the local Git repository. Exchanging commits has to be performed manually and explicitly.

Q4. Why is git diff used ?
ans:-
Diff command is used in git to track the difference between the changes made on a file. Since Git is a version control system, tracking changes are something very vital to it. Diff command takes two inputs and reflects the differences between them.

Q5. Can we leave the commit message as blank?
ans:-
 Yes , we can leave a commit message blank but writing message shows good development procedure and helps in keeping track on project.

*************************************************************************************************************************************************************************
*************************************************************************************************************************************************************************
Task Day_3:-
Q1.  What is meant by the term fork and clone?
 ans:-
  Fork- Fork is making a copy of the original repository, where the original repository remain same on the GitHub account. Forking is done in order to do some changes to someone's repository.
Clone:- Clone is making a copy of a repository in to the local machine.
cloning is done  in order to add any/some file(s) or edit any existing file in the cloned repository.
Changes made to the forked repository can be merged with the original repository via a pull request. 
Forking is a concept while cloning is a process. Forking is just containing a separate copy of the repository and there is no command involved. Cloning is done through the command ‘git clone‘ and it is a process of receiving all the code files to the local machine.

Q2. What are branches in Github?
ans:-
A branch is a version of your repository, or in other words, an independent line of development.
The purpose of branch or branches is to work on the repository on multiple aspects at the same time.
A repository can contain multiple branches, which means there are multiple versions of the repository. 
To create a branch one can use "git checkout -b branchname". This command will create a new branch switch to it.
After working/committing changes in branch we can merge the created branch to master branch in repository.
one can even commit changes in master branch and also on local branch and can merge it.

Q3. What is PR?
ans:-
  PR is PULL REQUEST. It is a request to original repository. It is a request to accept or pull the changes in the repository after forking it. 
It is the final step in producing a fork of someone else’s project.
Pull requests let you tell others about changes you've pushed to a GitHub repository. 

Q4. Can we delete the master branch if not Why?
 ans:-
yes, we can delete master branch.
we need to go to the GitHub page for our forked repository, and click on the “Settings” button.

Click on the "Branches" tab on the left hand side. There’s a “Default branch” dropdown list near the top of the screen.

From there, select placeholder (where placeholder is the dummy name for your new default branch).

Confirm that you want to change your default branch.

enter the command: "git push origin :master"

Q5. How can we delete a branch?
 ans:-
  Branches ccan be deleted "Locally" and "remotely".
 1. Locally:-
 2. Git will not let you delete the branch you are currently on so you must make sure to checkout a branch that you are NOT deleting. For example: git checkout master

Delete a branch with git branch -d <branch>.
The branch is now deleted locally.

2. remotely:-
we can use this command to delete a branch remotely:
 git push <remote> --delete <branch>.
The branch is now deleted remotely.

we can also use this shorter command to delete a branch remotely: git push <remote> :<branch>
*************************************************************************************************************************************************************************


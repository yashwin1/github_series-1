
TASK 1:

Q1. What do you mean by Git & GitHub?
Ans. Git:
-It is a distributed version control system.
- It's an open source tool to manage source code.
- It includes the concept of version control that let us manage and keep track on our source code history.
- one of the feature of Git is trunk based development.
GitHub:
- It's a web service.
- online service to which developers who use Git can connect & upload or download resources.
-lets you manage Git versions.
- anyone from open source to business github can be used anywhere.
- Although Github is free but if one if working for private business & don't want to open their code so they can go for private repositories where u have to pay a little amount.
Q2. Why Github is so popular and used in most projects?
Ans.
- It provides safe cloud storage for source code.
- Supports all programming languages.
- Provides wide exposure for our projects and for us.
Q3. What is VCS? How git is VCS?
Ans.
Version control system (VCS) tracks all the changes made to your code and who makes them.One can easily review the detailed changes
 history especially it is useful when one is working in collaboration in a project to keep a track.
Git is basically designed for coordinating work among programmers but can be used to track changes in any set of files.
Q4. what are other platforms similar to github?
Ans.
1. GitLab - You can import your GitHub repositories to GitLab.
2. BitBucket- This offers large file storage for game development and number of free private repositories.
3. LaunchPad- Fully free.
Q5. Why are you interested in learning of Git and Github?
Ans. During working on my academic project and other projects which uses Android studio I found it very difficult to save projects and versions and all..and 
to do changes to existing one all these kind of things creates a number of errors in Android studio . So, I get to know about the features of Git and GitHub..and 
I found it very interesting and helpful for my future projects and existing one's .


TASK 2:

Q1. How git workflow works?
Ans. There are 4 fundamentals of Git workflow:
1. Workspace - which is our local directory
2. Index- also called stage
3. Local Repository- HEAD
4. Remote Repository
If you consider a file in your workspace it can be in 3 possible states:
i. It can be committed which means latest changes to the file are safely stored in local repository .
ii. It could be modified and changes are not saved in local Repository so locally modified.
iii. It can be staged means that it can be considered in next commit.
Some commands :
1. add(-u): add file from workplace to index
2. commit: all files staged (one can also directly commit from workplace to local Repository)
3. push: pushes your changes from local Repository to remote Repository.
In case for opposite flow we use fetch command.
Q2. What are the different stages of a git project as commit ,add?
Ans. There are 3 stages:
1. Untracked: file exists but not part of git VCS.
2. Staged: file added to git VCS but changes not committed.
3. Committed: Changes committed . One can use git status command to know the current stage of files in repository .
Q3. Is it possible to do a git commit before git add. if you have made any changes. explain?
Ans. No, as we need to explicitly tell Git about the changes which we want to include so before commit command run git add command as file won't be automatically included when it is changed.
Q4. why is git diff used?
Ans.
- It tracks different changes made in a file.
- it only shows difference between your working copy and Repository.
-Shows exact one by one difference.
Q5. Can we leave a commit message as blank?
Ans. Yes , one can leave a commit message blank but writing message shows good development procedure and helps in keeping track on project.
Link to GitHub repository :
https://github.com/PriyanshiChamoli/git_series.git

Task 3:

Q1. What is meant by term fork and clone?
Ans.
Fork:
-Working on someone else project or using there project as starting point of your own is known as Forking.
- Creating a fork is producing a personal copy of someone else's project.
- Fork act as a sort of bridge between original Repository and your personal copy.
But after the process of forking project still remains on github after copying so we need to clone it to our computer.
Clone:
- Refers to creating a copy of an existing git repository in a new directory.
- This automatically creates a connection that points back to the original repository,  which makes it very easy to interact with the central repository.
Q2. What are branches in Github?
Ans.
-Git branch is the feature of Git which isolate development work without affecting other branches in Repository.
-People create different branches and work on different aspects of the same document.
- One can merge a branch into another branch using Pull request.
Q3. What is PR?
Ans.
- PR( Pull Request) let you tell others about changes you have pushed to a branch in a repository on Githib.
- Once a pull request is opened, you can discuss and review changes and add commits before your changes are merged into the base branch.
Q4. Can we delete the master branch if not why?
Ans. Yes , we can delete a master branch.
Steps:
 First you delete master in your local clone.
>To do that we first make a new branch called alpha or similar. and delete master from there.
Commands:
git branch alpha
git checkout alpha
git branch -D master
>Next delete branch on github. First we have to make github look at our alpha branch,then delete master.
i. Push up the alpha branch
Commands:
git checkout alpha
git push origin alpha
then set alpha to github default branch.Go to the main github page for your repository,  click "Admin" button . There is a " Default branch " dropdown list near the top of screen from there select alpha. On the interface I'm looking at, a green tick appear above the dropdown list.
Now, at command line:
git push origin: master
Q5. How can we delete a branch?
Ans.
Local and remote branches actually have nothing to do with each other .They are completely separate objects of Git.So we need to delete them separately.
1. Deleting local branch
$ git branch -d feature/ login
Note: If you want to delete a branch that contains unmerged changes use "-f" flag . Use this with care because it makes losing data very easy.
2. Deleting remote branch
$ git push origin --delete feature/login
---------------------------------------------------
PR Links:
https://github.com/codewayy/github_series/pull/74
https://github.com/PriyanshiChamoli/git_seres/pull/1

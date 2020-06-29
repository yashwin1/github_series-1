 Task no 1
Question 1. What do you mean by git and GitHub?
Answer:-Git is a version control system that lets you manage and keep track of your source code history. GitHub is a cloud-based hosting service that lets you manage Git repositories. If you have open-source projects that use Git, then GitHub is designed to help you better manage them. 

Question.2. Why GitHub is so popular and used in most of the projects? 
Answer:-GitHub is a Git repository hosting service, which provides a web-based graphical interface. It helps every team member to work together on the project from anywhere and makes it easy for them. Github is open source projects than any other code repository/version control platform in existence.GitHub is the world's largest software development platform. It supports all popular programming languages.

Question 3. What is a version control system? How Git is a VCS? 
Answer:-Version control systems are a category of software tools that helps record changes to files by keeping a track of modifications done to the code.Developers can compare earlier versions of the code with an older version to fix the mistakes.

Question 4. What are the other platforms similar to GitHub?
Answer:-1 Gitlab
2 SourceForge
3 Google Cloud Source Repositories
4 Apache Allura
5GitKraken

Question 5.Why are you interested in learning of Git and GitHub?
Answer:-Git is a free, open-source software distributed version control system (DVCS) designed to manage all source code history and GitHub is a web-based hosting service for Git repositories. It offers all of Gits DVCS SCM and has some additional features.Its interesting to learn about how to distributed version control works. That's why I am interesting to learn Git and GitHub


Task no. 2


Question A. How git workflow works?
Answer:-  1 workspace:-  which is our local directory
2 Index:- it's also called as stage 
3 Local Repository:-The local repo is on your computer for only your direct use.
4 Remote Repository:- The remote repo is typically elsewhere and for your indirect use.
Workspace file contains 4 state 
1 Root folder.
2 User name and email.
3 Set of remote repositories (so it is able to fetch it; see below)
4 Current list of commit bundles (changelists) and branches.
Few commands :-
a) git init:-(git init) 
This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.
b) git commit:-(git commit -m) 
Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.
c) git configuration:- (git config) 
With Git, there are many configurations and settings possible. git config is how to assign these settings.


Question B. What are the different stages of a git project as commit ,add?
Answer Untracked:- the file exists, but is not part of git's version control. 
Staged:- The file has been added to git's version control but changes have not been committed. 
Committed:- This is the final stage, as this stage finally applies the new changes to the remote repository.: the change has been committed. 


Question C. Is it possible to do a git commit before git add. if you have made any changes. Explain why?
Answer:- No, because according to the process
first, we have to add the file and then commit changes to it
After making the changes we will add them using “git add .”
and then we can commit it using (commit -a).

Question D. Why is git diff used?
Answer The main objective of version control is to enable you to work with different versions of files. Git provides a diff command to let you compare different versions of your files. The most common scenario to use diff is to see what changes you made after your last commit.Diff command takes two inputs and reflects the differences between them. These inputs don’t need to be filed only.


Question E. Can we leave a commit message as blank?
Answer:- yes, we can leave commit message as blank but if we provide meaningful message with this it's easy to understand  why change made and also it's good habit for developer to provide message. 

Link to GitHub repository:-
https://github.com/dhirajumate19/Git_Series

Hello everyone
I'm Dhiraj Umate currently pursuing B.Tech in
Bajaj Institutions of Technology, Wardha
Task no. 3

Question 1.What is meant by the term fork and clone?
Answer:-
forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.
A clone is a Git command line utility which is used to target an existing repository and download and existing git repository to your local computer.
Question 2.What are branches in GitHub?
Answer :-
Branching is a feature available in most modern version control systems. Branching in other VCS's can be an expensive operation in both time and disk space. In Git, branches are a part of your everyday development process. Git branches are effectively a pointer to a snapshot of your changes. When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes. This makes it harder for unstable code to get merged into the main code base, and it gives you the chance to clean up your future's history before merging it into the main branch.A branch represents an independent line of development. Branches serve as an abstraction for the edit/stage/commit process.
Question 3.What is PR?
Answer:-
Pull Requests are commonly used by teams and organizations collaborating using the  shared repository Modell, where everyone shares a single repository and topic branches are used to develop features and isolate changes. Many open source projects on GitHub use pull requests to manage changes from contributors as they are useful in providing a way to notify project maintainers about changes one has made and in initiating code review and general discussion about a set of changes before being merged into the main branch.

Question 4.Can we delete the master branch if not Why?
Answer:-
It is possible to delete Master branch just follow the  given below:-

       First you delete master in your local clone. To do this we first make a new branch called placeholder or similar, and delete master from there:
we will get an error. That is because github is looking at the master branch to provide the web content when you browse that repository. So we first have to make github look at our placeholder branch instead, then delete master.
First push up the placeholder branch:
git checkout placeholder  if not on placeholder already
git push origin placeholder

      Then set placeholder to be the github default branch. Go to the main github page for your forked repository, and click on the “Admin” button.

There’s a “Default branch” dropdown list near the top of the screen. From there, select placeholder. On the interface I’m looking at, a green tick appears above the dropdown list. Now you can do (from the command line):
git push origin :master
and - no master branch...

Question 5.How can we delete a branch?
Answer:-
a. deleting branch locally
This is the easy part since you're just working on the Git repository that you (presumably) own and control. Here is the command you'll likely need:
$ git branch -d <local_branch>

b. Deleting remote branch
In Git, local and remote branches are separate objects. Deleting a local branch doesn’t remove the remote branch.
To delete a remote branch, use the git push command with the -d (--delete) option:
git push remote_name --delete branch_name


PR links :-
1 https://github.com/dhirajumate19/Git_Series/pull/2
2 https://github.com/codewayy/github_series/pull/77
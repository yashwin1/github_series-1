### Task 1
1 . _Git is a distributed version control system  and also it is one of the Software. It is help to work on project simultaneously with different versions . Github is a web based hosting services for Git repository to bring teams together_ .

2. Git is popular because of...
_As the largest open source repository in the worldm GitHub offers a number of unmatched benefits to developers everywhere. GitHub is the world's largest software development platform. It supports all popular programming languages_
**1.The Largest shared Repository**
**2.Easy Version control** 
**3.Secure cloud storage**

3. _Git Version Control System. ... The version control system is a collection of software tools that help a team to manage changes in a source code. It uses a special kind of database to keep track of every modification to the code. Developers can compare earlier versions of the code with an older version to fix the mistakes_

4. Similar Platforms are ....
**1.Gitlab**
**2.SourceForge** 
**3.Cloud source Repositories**
**4.Apache Allura**

5. _GitHub is an open-source repository hosting service. It hosts our source code projects in a variety of different programming languages and keeps track of the various changes made to every iteration. Its interesting to learn about how to distributed version control works. Thats why I am interesting to learn Git and Github_.


## Task 2
Que A. How git workflow works?
Answer:-  _1 workspace:-  which is our local directory_
2 _Index:- it's also called as stage_. 
3 _Local Repository:-The local repo is on your computer for only your direct use_.
4 _Remote Repository:- The remote repo is typically elsewhere and for your indirect use_.
**Workspace file contains 4 state** 
**1 Root folder**.
**2 User name and email**.
**3 Set of remote repositories (so it is able to fetch it; see below)**
**4 Current list of commit bundles (changelists) and branches**.
Few commands :-
a) git init:-(git init) 
This command turns a directory into an empty Git repository. This is the first step in creating a repository. After running git init, adding and committing files/directories is possible.
b) git commit:-(git commit -m) 
Record the changes made to the files to a local repository. For easy reference, each commit has a unique ID.
c) git configuration:- (git config) 
With Git, there are many configurations and settings possible. git config is how to assign these settings.


Que B. What are the different stages of a git project as commit ,add?
Answer Untracked:- _The file exists, but is not part of git's version control. 
Staged:- _The file has been added to git's version control but changes have not been committed_. 
Committed:- _This is the final stage, as this stage finally applies the new changes to the remote_ repository.: _the change has been committed_. 


Que C. Is it possible to do a git commit before git add. if you have made any changes. Explain why?
Answer:- **No**, _because according to the process_
_first, we have to add the file and then commit changes to it_.
_The "commit" command is used to save our changes to the local repository. That we have to explicitly tell Git which changes we want to include in a commit before running the "git commit" command. This means that a file won't be automatically included in the next commit just because it was changed. Instead, we need to use the "git add" command to mark the desired changes for inclusion_._After making the changes we will add them using “git add_ .”
_and then we can commit it using (commit -a)_.

Question D. Why is git diff used?
Answer : _Git provides a diff command to let you compare different versions of your files_. _The most common scenario to use diff is to see what changes you made after your last commit_.Diff command takes two inputs and reflects the differences between them. These inputs don't need to be filed only.


Question E. Can we leave a commit message as blank?
Answer:- yes, we can leave commit message as blank but if we provide meaningful message with this it's easy to understand  why change made and also it's good habit for developer to provide message. 

Link to GitHub repository:-
https://github.com/sakshinathile/Git_Series


## Task No. 3 
Que :- Fork and Clone are two different things but those things are very popular on Git.
Fork :- Forking is we can take the copy of some one project in our system and make changes on it , will upload to the centralized server. The forked repository is mostly static. It exists in order to allow us to publish work for code review purposes. We don't do active development in our forked repository.
 
Clone :- The cloned repository is our active repo. It is where we do all your work. But other people generally don't have access to our personal cloned repo, because it's on our laptop. So that's why we have the forked repo, so we can push changes to it for others to see and review.


Que 2. :- The way git, and GitHub, manage this  especially when more than one person is working in the project and making changes is by using branches. A branch is essentially is a unique set of code changes with a unique name. Each repository can have one or more branches. Master is the default branch..The main branch — the one where all changes eventually get merged back into, and is called master. This is the official working version of our project, and the one we see when we visit the project repository .

Que 3 :- Pull requests is changes we've pushed to a GitHub repository. Once a pull request is sent, interested parties can review the set of changes, discuss potential modifications, and even push follow-up commits if necessary.
Pull Requests are commonly used by teams and organizations collaborating using the Shared Repository Model, where everyone shares a single repository and topic branches are used to develop features and isolate changes. Many open source projects on Github use pull requests to manage changes from contributors as they are useful in providing a way to notify project maintainers about changes one has made and in initiating code review and general discussion about a set of changes before being merged into the main branch.

Que 4 :- Yes but it is too difficult to remove the master branch . I'm not using the master branch and each time I write git status it tells me how far ahead my branch is from the master.
When I try to delete the master branch git branch -d master it deletes it only on my local repository and not on the remote git server.

Que 5:  We can delete the branch by two ways ..

a. Delete the branch Locally.

The -d option will delete the branch only if it has already been pushed and merged with the remote branch. Use -D instead if you want to force the branch to be deleted, even if it hasn't been pushed or merged yet.

The branch is now deleted locally.

Deleting a branch REMOTELY
Here's the command to delete a branch remotely: git push <remote> --delete <branch>.

For example: git push origin --delete fix/authentication

The branch is now deleted remotely.

PR links 

1.https://github.com/sakshinathile/Git_Series/pull/2

2.https://github.com/codewayy/github_series/pull/78
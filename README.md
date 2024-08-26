# GIT

## What is GIT?

Open source software which was created in 2005 by a set of Linux developers.
It is the most popular and widely used, distributed version control system out there now wide distributed because it allows software developers across the world to work on a single project together.
So it enables developers to work on the project as a team and collaborate remotely.

## What is a Version control system?

A version control system enables multiple software developers to work on a single project together.
The version control system enables this by keeping a track of the history of changes.
A version control system, enables developers to see every changes.

    * who made those changes
    * what were those changes
    * why those changes were made
    * when were those changes made

## Features of Git

**Opensource** – Git is open source and is licensed under GPL.

**Easy to use** – Git is very easy to learn and use for developers.

**Distributed** – Git is distributed, which means it allows the software developers across the world to work on a single project.

**Rollback mistakes** – Git allows you to save checkpoints in the form of commits.

## Benefits of Git

    * Saves time
    * Undo mistakes
    * Track changes
    * Easy to use
    * Makes collaboration easy

## Repository

A Repository is a collection of files and folders associated with the project. So every project has a git repo associated with it.

## Commit

Git allows you to store multiple versions of files and keep a track of changes. Git commit basically saves a snapshot of your repository, which you can even revert to in future.

## Branch

Using a git development can be organized into multiple lines of development called branches. Whatever changes a developer does in a branch does not impact or reflect other branches unless its mergerd.

## Push

Once you have committed the changes locally you need to push changes to the remote server. So that they are stored in a safe way.

## Pull

Pull is an action that is performed if the local repository that you have on your machine does not have some recent changes that other developers added onto the remote server.

## How Git works

![Workflow](images/workflow.png)

## GIT Commands

**`git add <filename>`**  → This adds a file into staging area

**`git commit <commit-message>`** →This commits the changes that have been done

**`git init`** → This initializes a new git repository and begins tracking it

**`git push`** → Pushes changes to the remote server like github, gitlab, bitbucket, etc

**`git status`** → Show the status of git on your machine.

**`git pull`** → Pulls update from the remote server to your local machine

# GitHUB

## What is GitHub?

* GitHub is the most popular code hosting service that allows developers to host a coding project or a repository and also allows them to track the changes.

* So GitHub is nothing but a service that developers can work with to save their coding project and also to keep track of these changes.

## Features of GitHub

* Store your code in cloud
* Track changes
* Collaboration between developers
*  Way to create pull requests
* Integrated issue and bug tracking
*  Track and assign task

## Repositories on GitHub

Repositories on GitHub are two types,

1) Public
2) Private

**Public**: Public repositories can be accessed by anyone in the world.

**Private**: Private repositories can only be accessed by a specific set of people who have been given access to that particular repository.

## Assets of GitHub

* GitHub is easy to learn and widely used. It also offers an excellent documentation for its users.

* You can easily set up your development portfolio on GitHub and show off your work to the recruiters.

* GitHub allows you to host your code on a remote server. So if your local machine crashes, you have everything available on GitHub.

## Getting Started - Installing Git

[Getting Started - Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

## Configure GIT

1) In Cloud Shell, to double-check that Git is installed, type git --version
```
git --version
```
2) You should see output that looks something like this example:

```
git version 2.7.4
```

3) To configure Git, you must define some global variables: user.name and user.email. Both are required for you to make commits.

4) Set your name in Cloud Shell with the following command. Replace `<USER_NAME>` with the user name you want to use.
```
git config --global user.name "<USER_NAME>"
```
5) Now, use this command to create a user.email configuration variable, replacing `<USER_EMAIL>` with your e-mail address:

```
git config --global user.email "<USER_EMAIL>"
```
6) Run the following command to check that your changes worked
```
git config --list
```

7)  Confirm that the output includes two lines that are similar to the following example. Your name and e-mail address will be different from what's shown in the example.
```
user.name=santhoshbabu0411
user.email=santhoshbabu0411@gmail.com
```

## Setting up Git Init

![git-init](images/Git-init.png)

## Adding Files to staging area

In Git, before you commit your changes, you need to add your files to the staging area. There are two main ways to do this:

**Adding a Specific File**

```
git add <filename>
git add index.html
```
**`Why Use It?`**: This is useful when you only want to add certain files to the commit.

**Adding All Changed Files**
Use this command to stage all the changed files in your directory:
```
git add .
```

**`Why Use It?`**: This is quick and adds everything that’s been changed, but be careful—it might add things you didn’t intend to commit.

## Example:
![git-init](images/Adding-files-staging-area.png)

## Unstaging Files in Git

Sometimes, after adding files to the staging area, you might realize you don’t want to include them in your next commit. You can unstage these files using the following commands:

```
git reset <file-name>
git reset index.html

git rm --cached <filename>
git rm --cached index.js
```
* Use git reset `<file-name>` to unstage a file while keeping your changes.
* Use git rm --cached `<file-name>` to unstage a file and stop tracking it in Git, but keep the file locally.


## Commit

**`Snapshot of Changes`**: A commit records the changes you’ve made to your files since the last commit. It’s like taking a picture of your project’s current state.

**`Unique Identifier`**: Every commit has a unique ID, so you can easily refer back to it later.

**`Commit Message`**: When you create a commit, you add a message describing what changes you made. This helps you remember what you did and why.

**`Permanent Record`**: Commits are saved in your Git repository, meaning you can always look back at your project’s history.

## Example:

![git-init](images/commit.png)

## Seeing changes in git

![git-init](images/Seeing-changes-in-git.png)
![git-init](images/changes-on-github.png)

## Amending Commits

Amending a commit in Git allows you to modify the most recent commit you’ve made. This is useful if you forgot to add some changes, want to correct your commit message, or need to update the commit content.

## Example:

![git](images/Amend.png)

## Git Push

When you push your commits, you’re essentially transferring the changes from your local Git repository to a remote repository. This allows others to see your work, collaborate, or deploy the code from the remote repository

## Example

![git](images/Git-push.png)

## Git Pull

When you run git pull, it updates your local branch with the latest commits from the corresponding branch in the remote repository. This is how you get the most up-to-date version of the code that others might have pushed to the repository.

## Example
**`Note`** I added a README file to my GitHub repository and committed it. Then, I noticed that the README file wasn't present in my local repository, so I pulled the code to receive the README file locally

![git](images/Readme-file-pull.png)
![git](images/Readme.png)
![git](images/Git-pull.png)

## Branches

A branch in Git is like a separate workspace within your project, where you can work on new features, bug fixes, or experiments without affecting the main code

## Why Use Branches?
**`Isolate Work`**: You can make changes on a branch without impacting the main project.

**`Safe Experimentation`**: Try out new ideas on a branch without risking the stability of your main code.

**`Team Collaboration`**: Multiple people can work on different branches simultaneously without conflicts.

## Example

![git](images/B1-Github.png)
![git](images/Branch.png)
![git](images/B2-Github.png)

## Deleting a branch

Deleting a branch in Git helps tidy up your repository after you’ve completed a feature or bug fix. Once a branch is merged into the main branch, it can be safely removed as it's no longer necessary.

## Example

![git](images/Deleting-Branch.png)


## Merging Branches in Git

Merging branches in Git combines the changes from one branch into another. It’s commonly used to bring the updates from a feature or bug fix branch into the main branch after the work is complete.

## Example

![git](images/Merge-dev-prev.png)
![git](images/Merge-main-prev.png)
![git](images/Git-Merge.png)
![git](images/Merge-main-after.png)

## Handling Conflict

A merge conflict occurs in Git when two branches have made changes to the same part of a file, and Git cannot automatically determine which change to keep. Here's a breakdown of how conflicts arise and how they are handled:

## How Conflicts Arise

* **`Concurrent Changes`** : If two branches make changes to the same line in a file, Git cannot decide which change to keep during a merge.

* **`Overlapping Changes`** : Conflicts also occur if one branch modifies a file and another branch deletes or renames it.

## Example

![git](images/conflict/Group-7241.png)
![git](images/conflict/3.png)
![git](images/conflict/Group-7240.png)
![git](images/conflict/7.png)


## Stash and Pop

**`Stashing Changes`**:

When you're in the middle of working on something and need to switch branches or pull in new changes without committing your current work, you can "stash" your changes. This saves your modifications (tracked files, staged changes, and optionally untracked files) and reverts your working directory to the last commit.

**`Popping Stashed Changes`**:

Once you're ready to return to your stashed work, you can "pop" the stash. This restores the saved changes back to your working directory.

## Example

![git](images/stash-pop.png)


## Clone

The git clone command is used to create a copy of a remote repository on your local machine. 

## Example

![git](images/git-clone-github.png)
![git](images/git-clone.png)






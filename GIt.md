# GIT

## What is GIT?
What is Git?

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
**`Why Use It?'**: This is useful when you only want to add certain files to the commit.

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






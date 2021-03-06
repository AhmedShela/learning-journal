# **git**

### What is the Ideal of Git?

The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). This system entails a single server storing all changes and file versions, which can be accessed by various clients. This streamlined the collaboration process (by eliminating the need to involve all local databases), allowed programmers to have more knowledge of team members’ activities with certain files, and gave administrators much more control over divvying up revision privileges

### snapshot
Git stores a reference for every each time you saved a changed version of your project

### local operations
git allow one to continue work on a project even when not online

### tracking chages
Git will always detect file corruption or loss of information in transit.

### Loss of Data
Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

![loos of data](https://www.udemy.com/blog/wp-content/uploads/2015/08/image066.png)

## start with Git
* after installing get you should configer Git using this code
`git config`

* and then start identity setting using this set of codes

`git config --global user.name "Jane Smith"`

`git config --global user.email "example@email.com"`

* To confirm that you have the correct settings, enter the following command:

`git config --global user.name (should return Jane Smith)`

`git config --global user.email (should return example@email.com)`

* then you should set the defult text editor using this code

`$ git config --global core.editor emacs`

* finaly using this code you can check out you settings
`git config --list`

### Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

`$ cd test (cd = change directory)`
Use the git init command`
`$ git init`
*Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.*

* To start tracking these repository files, perform an initial commit by typing the following:
`$ git add *.c`
`$ git add LICENSE`
`$ git commit -m “any message here”`
Now, your files are tracked and there’s an initial commit. We will discuss the particular commands in detail soon.

### Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

`$ git clone https://github.com/test`

### Local Repository Structure
The local Git repository has three components:

* Working Directory: The actual files reside here.
* Index: The area used for staging
* Head: Points to the most recent commit

![Local Repository Structure](https://www.udemy.com/blog/wp-content/uploads/2015/08/image036.png)

### Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

Tracked

Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

Untracked

Untracked files were not in the last snapshot and do not currently reside in the staging area.

* After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

### The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit.
You stage the modified file.
Then, you commit staged changes.

Check File Status
To determine the state of files, utilize the git status command:

`$ git status`

Tracking and Staging a New File
Single File

Track one file only by using the following format:

git add filename
All Files

Track all files in a repository by using the following command:

`$ git add *`
*After using these commands, files are tracked and staged for committing.

After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the git status command:

`$ git status`

On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage)
new file: EXAMPLE
This information tells us that there are changes to be committed and that the file has been staged.

Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

`$ git commit -m “made change x,y,z”`
* This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

Committing All Changes
`$ git commit -a`
* This command commits a snapshot of all modifications to tracked files in the working directory.

Pushing Changes
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

`$ git push origin master`
This command pushes changes from the local “master” branch to the remote repository named “origin”.


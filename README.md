# Learning how to use GitHub

### Objectives

* Store version-controlled projects online
* Work with collaborators on the same project

### Not covered

* Command-line git tools
* Working with branches

### Required

* GitHub GUI ([Windows](https://windows.github.com/), [Mac](https://mac.github.com/))
* GitHub account
* Good text-editor (e.g. Atom or Sublime)
* Internet connection

### Instructions

#### A. Making changes

Basic git usage is to have a repository online, make changes to a local copy on your machine, and then push those changes to the online version. This allows you to have a backup of all your code, have a history of all the steps you've taken for developing your code (which allows you to revert to previous version if anything goes wrong) and work with collaborators.

>*Repo* -- or repository is a folder that is under version-control. It can be held online and across multiple computers, each copy is kept up-to-date by syncing. When under version-control, nothing is ever lost. All versions and deleted files are kept in the `.git/` folder.

**1. Fork this repo**

Every repo on GitHub can be forked. Look for the fork button in the top right corner of this page to copy this repo to your own account.

>*Fork*  -- copy someone else's repo to your own account.

**2. Clone this repo to your local machine**

In your GitHub GUI, select the + sign in the top-left corner. And clone the recently forked repo. This will create a complete copy of the repository on your machine.

>*Clone*  -- copy a repo, to which you have access, to your own computer.

**3. Make a change to the poem.**

With the repo on your machine, you can now make changes to it. Open the `script.md` file and adapt the poem to your liking. Or if you want to write your own poem or anything else, add anything to `script.md`.

**4. Commit and sync this repo**

Now you've made a change to `script.md`, you'll see the GUI tell you what changes you have made. Commit your change with a message e.g. "I made the poem better". Then click the sync button in the top-right corner and check your copy online: `https://github.com/[YOUR ACCOUNT NAME]/Teaching-github`. Also check our the history of `script.md` online or on your GUI.

>*Commit*  -- A change with a message (e.g. corrected infinite loop in myscript.sh) that can then be pushed to GitHub. All changes made must be committed in order to sync them.

#### B. Ignoring files

Git will version control everything placed in the repo. This is not always helpful as you do not necessarily want all files and folders to be synced and not everything needs to be under version-control (e.g. automatically generated files). To control what is under version-control use the `.gitignore` file.

>*.gitignore* -- a text file that contains a list of files (or file patterns) that should be ignored.

**1. Open the .gitignore and ignore .csv files**

In your text editor, open the `.gitignore` file and add `*.csv` under 'Ignored files'. This tells git to ignore any file that ends with `.csv`. It is useful to ignore data files (like csv files) for multiple reasons: GitHub has a 1GB repo limit; it is pointless version controlling files that are automatically generated, this will make the `.git/` folder very large over time and slow-down simple git processes; it will reduce the amount of bandwidth used when performing simple tasks like cloning and syncing.

Now you've edited a file, commit it with a message in your GUI e.g. 'Now ignoring csv files'

>*.DS_Store* -- in the .gitignore you will already find a file name. This is a Mac generated file, it is not part of the coding project and should be ignored. The file helps Macs perform spotlight searches.

**2. Add a .csv file to the repo**

Create a new file in the repo called 'test.csv'. Does the git detect it?

>*. prefix* -- in UNIX systems this makes a file invisible. If you cannot find your `.gitignore` open a terminal and use `ls -a` to see all files in a folder. You can also use a simple terminal text editor like nano to modify the file (`nano .gitignore`).


#### C. Working with collaborators

1. Go to settings, add a collaborator
2. Force a merge conflict
3. 
Here are some changes that I hope will force a conflict

# GIT
These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   restore    Restore working tree files
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   diff       Show changes between commits, commit and working tree, etc
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   backfill   Download missing objects in a partial clone
   branch     List, create, or delete branches
   commit     Record changes to the repository
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   reset      Reset current HEAD to the specified state
   switch     Switch branches
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

# git status
   It is used to view the status of your git repositry.
   we can also use: git status -s
      This will show you a summary of the changes made to the status of your git repository.
# Using git add
syntax: git add file_name.extension
This command stages the untracked files.
To stage all the untracked files use:
         git add -A

# git restore
git restore --staged <file>...
to unstage staged files

# Using git commit
syntax: git commit -m "commit message"
                     OR
        git commit
      After pressing Enter right after typing this, the VIM Editor will open then to Insert your commit message.
      You have to first press 'I' key on the keyboard to insert, then you can procced to type your commit message.
      That will be seen in the top right corner.
      Once you're finished with your message, you have to exit the VIM editor by clicking esc, then in the bottom rigt you'll see the --INSERT-- written over there disappears and a blanck space is there.
      Now you have to click on shift + ; to type :, then type wq in assosiation with it.
      Now, as you hit the enter button you'll exit the VIM editor.
      And you've successfully inserted your commit message.
To directly commit and skip the staging area:
   git commit -a -m "commit_message"

# Create files using git bash
use touch command to create new files
syntax: touch file_name.extension
      e.g; touch .gitignore

# Zoom IN and Zoom OUT
use: 'ctrl + + ' to zoom in
   And 'ctrl + - ' to zoom out

# Using git checkout
syntax: git checkout file_name.extension
This command will recover the mentioned file, and matches it to your last commit status.
OR for more than one file you have to use:
      git checkout -f
It will sync all your files in the given git folder to your last commit status.

# git log
syntax : git log
This command will show you the logs and details of all your git commits.
In the bottom left a cursor will blink after : , where you will press Q. to continue to your terminal.
To know in particular about the few last commits, use
   git log -p -number_of_commits (numeric form)

# git diff
syntax : git diff
It compares your working directory from staging area. Once you add all you changes to staging area then git diff will not show anything.
If you want to compare your working directory to your last commit, then use;
   git diff --stage

# Removing a file in git

syntax:  git rm file_name.extension
      It will delete the file from your working directory as well as from your staging area.
syntax: git rm --cached file_name.extension
      It will remove that file from your staging area.
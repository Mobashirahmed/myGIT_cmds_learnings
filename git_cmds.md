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

# Using git add
syntax: git add file_name.extension
This command stages the untracked files.
To stage all the untracked files use:
         git add -A

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
#### First time git setup
git config --global user.name "Prasad Addagarla"
git config --global user.email <>
git config --global core.editor gvim/emacs/vim
##### to list all configurations already in the git config
git config --list 

#### If you are starting to track an existing project in Git you need to go to project's directory and type
 git init
#### cloning an existing repository
 git clone url loacl path
#### Checking the status of your repository
 git status
#### How to stage new files
 git add filename
#### How to make git ignore some files
 cat .gitignore
 modify the file .gitignore to add regular expressions that match with the names of the files to be ignored
* Blank lines or lines starting with # are ignored.
* Standard glob patterns work.
* You can end patterns with a forward slash (/) to specify a directory.
* You can negate a pattern by starting it with an exclamation point (!).
* # a comment - this is ignored
* *.a # no .a files
* !lib.a # but do track lib.a, even though you're ignoring .a files above
* /TODO # only ignore the root TODO file, not subdir/TODO
* build/ # ignore all files in the build/ directory
doc/*.txt # ignore doc/notes.txt, but not doc/server/arch.txt
# To see what you’ve changed but not yet staged, type git diff with no other arguments
git diff filename
# If you want to see what you’ve staged that will go into your next commit, you can use git diff --staged
git diff --staged filename
# Remember a file that is staged and them modified can be listed in bothe staged and modified sections
## to see what you have already staged but not what you have modified run
git diff --cached filename
# To commit your changes 
git commit
## To skip the staging step when there are a lot of modified files you can use the -a option with git commit
git commit -a
## To add a message to the commit use -m in the command line
git commit -a -m "My commit"


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

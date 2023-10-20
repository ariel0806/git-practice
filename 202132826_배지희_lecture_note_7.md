
## 202132826_배지희_lecture_note_6

## Git

## Git config: First-time setup
$ git config --global user.name "ariel"
$ git config --global user. email ariel@gachon.ac.kr
$ git config --global init.defaultBranch main
$git config --list
$ git config --list --show-origin
$ git config user.name
ariel


## git init
- Intializing a repository in an existing directory

$ git init
Initialized empty Git repository in /gome/ariel/OSS/transformers/.git/
$ls -lha
total 64K
drwxrwxr-x 3 ariel ariel 4.0K 10월 4 14:48
.....기타등등


## git status
- checking repository Status

$ git status
On branch master
No commits yet
Untracked files:
(use "git add <file>..." to include in what will be committed)
    README.md
    기타등등
    
nothing added to commit but untracked files present (use "git add" to track)



## git add [file_name]
- Adding a new file to be staged

$ git add README.md
$ git status
On branch master
No commits yet
changes to be committed:
    (use "git rm --cached <file"..." to unstage)
        new file: README.md
Untracked files:
(use "git add <file>..." to include in what will be committed)  
     파일명들..
     
$ nano words. txt
->
university
class
home..


## git rm-cached[file_name]
- Unstaging a file

$ git rm --cached gistory_command.txt
rm 'history_command.txt'
$git status
On branch master
No commits yet
Changes to be committed:
    (use "git rm --cached <file> ..." to unstage)
    new file: README.md
untracked files:
    (use "git add <file>..." to include in what will be committed)
    gistory_command.txt
    
$ls history_command.txt
history_command.txt


##nano. gitignore
- Ignoring a file


## $ git commit -m "commit message"
- commit

$git commit -m "initial commit"
[maste (root-commit) 4b0c4f3] initial commit
9 files changed, 179 insertions(+)
create mode 100644 .gitignore
기타등등
$ git status
On branch master
nothing to commit, working tree clean


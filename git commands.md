# Config commands

`git config --global user.name "Name Surname"`

`git config --global user.email "some@mail.com"`

`git config --global init.defaultBranch <name>`  
 - change default branch name, normally **master**

`git config --global -e`
 - list/modify all added info
 - to modify info press A
 - to save & quit press ESC then :wq!

`git config core.autocrlf true`
 - in case of a misunderstood character

## Alias

[Source](https://gist.github.com/Klerith/0acf18bbece7923bcac55edb71b03c2b)

This configures customized commands, the general format to write an alias is:

`git config --global alias.<desired alias> <command>`

### Some useful aliases:

 - git lg:

`git config --global alias.lg "log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all"`

 - git s:

`git config --global alias.s "status --short"`

 - git s2:

`git config --global alias.s2 "status -sb"`

# Basic commands

`git init`
 - starts the proyect and creates the folder '.git' on current folder

`git status`
 - gives information on repository status, current branch, staged files and modified files.

`git add <filenames>`
 - adds filename(s) to staged changes

`git reset <filename>`
 - unstage file from **commit**

`git add .`
 - adds all modified files to **commit**

`git commit -m "Commit message"`
 - create a **commit** with staged changes

`git commit -am "Commit message"`
 - Combines `git add .` + `git commit -m "message"` to one command, ignores untracked files.

`git checkout -- .`
 - restore proyect to last commit

`git log`
 - shows commits info (author, date, time, branch and current head)

# Branches

`git branch`
 - check current working branch

`git branch -m <oldName> <newName>`
 - change branch name


# Additonal notes
When you want to keep an empty folder add an empty file named `.gitkeep`


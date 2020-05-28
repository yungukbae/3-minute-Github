# 3-minute-Github
How to upload and using Git command

Fisrt: Git install check

Windows Git install:https://git-scm.com/

Git install check(Mac OS, Linux)
$ git version
git version 2.xx.x

If the version does not come up

install git through each command

Fedora, RHEL, CentOS
$ sudo dnf install git-all

Ubuntu
$ sudo apt install git-all

Mac OS(Using Homebrew)
$ brew install git

Second: Local directory setting
$ cd {project directory}
$ git init

Name and Email setting
$ git config --global user.name "github name"
$ git config --global user.email "github email"

check 
$ git config --list

Third: Github repository connect
$ git remote add "name(anything you want)" "repository url or ssh"

check
$ git remote


Fourth: pull and push repository
$ git pull "name" master

$ git add [file name]
$ git commit -m "commit message"
$ git push "name" master

Done!
-----------------------------------------------------------------------------
How to resolve Git Permission denied(publickey)

$ ssh-keygen -t rsa -C "git email"

when password setting done

$cat /User/~skip~/id_rsa.pub
copy ssh-rsa to end 

Open Setting page at GitHub and go click ssh and GPG keys

Add your copy ssh key and test git push

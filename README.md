# 3-minute-Github
How to upload and using Git command
=====================================

## 1. Git install check
----------------------
Windows Git install:https://git-scm.com/

Git install check(Mac OS, Linux)
<pre><code>$ git version
</code></pre>
git version 2.xx.x

If the version does not come up

install git through each command

Fedora, RHEL, CentOS
<pre><code>$ sudo dnf install git-all
</code></pre>
Ubuntu
<pre><code>$ sudo apt install git-all
</code></pre>
Mac OS(Using Homebrew)
<pre><code>$ brew install git
</code></pre>
----------------------
## 2. Local directory setting
----------------------
<pre><code>$ cd {project directory}
</code></pre>
<pre><code>$ git init
</code></pre>

Name and Email setting
<pre><code>$ git config --global user.name "github name"
</code></pre>
<pre><code>$ git config --global user.email "github email"
</code></pre>

check 
<pre><code>$ git config --list
</code></pre>


----------------------
## 3. Github repository connect
----------------------
<pre><code>$ git remote add "name(anything you want)" "repository url or ssh"
</code></pre>

check
<pre><code>$ git remote
</code></pre>

----------------------
## 4. pull and push repository
----------------------
<pre><code>$ git pull "name" master
</code></pre>
<pre><code>$ git add [file name]
</code></pre>
<pre><code>$ git commit -m "commit message"
</code></pre>
<pre><code>$ git push "name" master
</code></pre>


Done!
-----------------------------------------------------------------------------
How to resolve Git Permission denied(publickey)
<pre><code>$ ssh-keygen -t rsa -C "git email"
</code></pre>

when password setting done
<pre><code>$ cat /User/.../id_rsa.pub
</code></pre>

copy ssh-rsa ~ end 

Open Setting page at GitHub and go click ssh and GPG keys

Add your copy ssh key and test git push

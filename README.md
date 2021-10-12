# Scaffold
This is a project scaffold for Python

## To create a new project from Terminal:
* Create a new repo on GitHub with Readme and Python gitignore
* Select code dropdown for new repo and link for SSH link
## Create a SSH key
* Type: ssh-keygen -t rsa
* Copy location for public key 
* eg: cat /home/ec2-user/.ssh/id_rsa.pub
* Copy public key and save in GitHub Settings in SSH keys with the same name as repo
## Clone repository
* Checkout git repo in Terminal: git clone git@github.com:machinatoonist/scaffold.git
## Create new files
* CD into the new project folder and make the following files:
* $ touch Makefile
* $ touch hello.py
* $ touch test_hello.py
* $ touch requirements.txt
* $ git remote -v
## Create new virtual environment using the same name as the repo
* $ python3 -m - venv ~/.scaffold
* Activate this environment
* $ source ~/.scaffold/bin/activate
* Run all the commands in the Makefile
* $ make all
## Save files to GitHub
* When finished push to GitHub
* $ git status
* $ git add *
* $ git status
* $ git commit -m "adding initial structure"
* Set tracking for first time use:
* $ git config --global user.name "Your Name"
* $ git config --global user.email you@example.com
* After doing this, you may fix the identity used for this commit with:
* $ git commit --amend --reset-author
* $ git push

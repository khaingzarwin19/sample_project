git & github
git is a popular version control system (VCS)

Difference Between Git and GitHub see: https://www.geeksforgeeks.org/difference-between-git-and-github/

1.Installing Git
#Window
see: https://gitforwindows.org/

#Mac
brew install git
Ref: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

2.First-Time Git Setup
List configuration
$ git config --list --show-origin
Setup
$ git config --global user.name 'user1'
$ git config --global user.email example_user@gmail.com
Checking configuration file
#Window
C:\Users\$USER
or
[path]/etc/gitconfig

# Mac
$cat ~/.gitconfig
Checking Your Settings
git config --list
ref: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

3.Adding a project to GitHub
#1: Create a folder for this project on your local
$ mkdir my-project

#2: change into this folder
$ cd my-project

#3: initialize a new, empty Git repository here
$ git init


#4: create readme file, then add all changes to the next (= first) commit
$ git add .

#5: create this first commit
$ git commit -m "Initial commit"

#6: Create a new repository on GitHub.com
![Getting Started](./images/create_new_repo.png)


![Getting Started](./images/quick_setup.png)


#7: add repository to local project & push to github
$ git remote add origin git@github.com:hha-m/my-project.git

$ git push -u origin master
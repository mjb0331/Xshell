git config --global user.name "Your Name Here"
# Sets the default name for git to use when you commit

git config --global user.email "your_email@youremail.com"
# Sets the default email for git to use when you commit

mkdir ~/Hello-World
# Creates a directory for your project called "Hello-World" in your user directory


cd ~/Hello-World
# Changes the current working directory to your newly created directory


git init
# Sets up the necessary Git files

# Initialized empty Git repository in /Users/you/Hello-World/.git/

touch README
# Creates a file called "README" in your Hello-World directory


git add README
# Stages your README file, adding it to the list of files to be committed


git commit -m 'first commit'
# Commits your files, adding the message "first commit"


git remote add origin https://github.com/username/Hello-World.git
# Creates a remote named "origin" pointing at your GitHub repo


git push origin master
# Sends your commits in the "master" branch to GitHub

git clone https://github.com/username/Spoon-Knife.git
# Clones your fork of the repo into the current directory in terminal

cd Spoon-Knife
# Changes the active directory in the prompt to the newly cloned "Spoon-Knife" directory

git remote add upstream https://github.com/octocat/Spoon-Knife.git
# Assigns the original repo to a remote called "upstream"

git fetch upstream
# Pulls in changes not present in your local repository, without modifying your files

git push origin master
# Pushes commits to your remote repo stored on GitHub


git fetch upstream
# Fetches any new changes from the original repo

git merge upstream/master
# Merges any changes fetched into your working files
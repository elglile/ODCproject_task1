git commande here

git clone https://github.com/elglile/ODCproject_task1.git # Clone the Repository

cd ODCproject_task1 #Enter folder

# Initialize git in your project directory
git init

# Create the Task1 folder and README.md file
mkdir Task1
echo "This is Task1 README" > Task1/README.md

# Stage and commit the changes
git add Task1/README.md
git commit -m "Add Task1 folder with README.md"
git status

# Push changes to GitHub
git push 
git status

# Create and switch to the dev branch:
git checkout -b dev

# Create a test file (e.g., test.txt), add it, and commit and push:
echo "Test content" > test.txt
git add test.txt
git commit -m "test fill in dev bransh"
git push -u origin dev
get status

# Create and switch to the %elg-new_feature branch:
git checkout -b %elg-new_feature

# create , add and push README.md fill
echo "Readme fill">README.md
git add README.md
git commit -m "add readme fill in %elg-new_feature bransh"
git status
git push -u origin %elg-new_feature
git status

# Create , add and push .gitignore fill 
echo ".">.gitignore
git add .gitignore
git commit -m ".gitignore fill"
git push -u origin %elg-new_feature

# Commit and Push Changes to GitHub Repo
git commit -am "Some changes"
git push

# merge my bransh whit dev bransh and the dev bransh whit main bransh
git merge dev
git checkout dev
git merge main

# Checkout to %USERNAME-new_feature, Make Changes in README.md and Commit
git checkout %elg-new_feature
echo "merge withdev branch">>README.md
git commit -am "update in README.md"


#  Check Your Repo with git log, Create log.txt, and Save Output
git checkout main
git log>log.txt
git add log.txt
git commit -m 'git log output'
git status
git push

# Delete Local and Remote %USERNAME-new_feature Branch
git branch -D %elg-new_feature
git push origin --delete %elg-new_feature
git status

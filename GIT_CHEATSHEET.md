# Git cheat sheet for this project

## Setup
git config --global user.name "Tabitha Khadse"
git config --global user.email "tabitha@ieee.org"

## Initialize and first commit
git init
git status
git add index.html
git commit -m "Initial commit"

## History and diffs
git log --oneline
git diff
git show

## Amend and soft reset
git commit --amend
git reset --soft HEAD~1

## Branch and switch
git branch feature_table
git switch -c feature_table
git switch main

## Merge and conflicts
git merge feature_table
# edit files to resolve
git add index.html
git commit -m "Resolve conflict"

## Remotes
git remote add origin https://github.com/tabitha-dev/html-repo.git
git branch -M main
git push -u origin main
git push

## Stash and cleanup
git stash push -m "WIP"
git stash list
git stash pop
git branch -d feature_table
git push origin --delete feature_table

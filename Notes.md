
## Initialize repository
git init 

## Status of repository
git status

## Stage file
git add index.html 

## Repo history (Shows only commits)
git log

## Configure git (global)
git config --global user.name "Your Name"
git config --global your.email@example.com

## Stage 2 files
git add orange.html blue.html

## Git log in one line (Condensing logs)
git log --online
git log --online blue.html

## View an old revision
git checkout 9dbfbda

## Return to current version
git checkout master

## Tag a release
git tag -a v1.0 -m "Stable version of the website"

## Return to stable release
git checkout v1.0

Note: After seeing the stable version of the site, we decide to  scrap the crazy experiment. But, before we undo the  changes, we need to return to the master branch. If we  didn’t, all of our updates would be on some non-existent  branch. As we’ll discover next module, you should never  make changes directly to a previous revision.  
git checkout master
git log --oneline

## Undo commited changes
git revert 56a3612

## Changing all tracked files to match most recent commit
git reset --hard
### Deleting un tracked files
git clean -f 

## Branches
Notes: 
1. error-proof method for changes in code
2. Store all experiments in a single directory
3. Standardizing workflow and collaboration

git branch
git branch crazy ## Create a new branch
git checkout crazy

## Renaming file
### rm command tells git to stop tracking
git rm crazy.html

## Delete a branch
git branch -d css
git branch

## Rule-of-thumb for git branches:
1. Create a branch for each major addition to the project
2. Don't create a branch if you can't give it a specific name

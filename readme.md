# Git Commands

## Git Init
- git init

## Git clone
- git clone girRemoteUrl

## Git Fetch
- git fetch -p //Remove if deleted from remote

- git fetch -all // all branch fetch


## Git Add existing repo
- git remote add origin remoteUrl


## Git commit && push
- git add .

- git commit -m "Commit message"

- git push

## Git Revert last commit
- git revert f4391b2

## GIT RESET COMMIT
- git reset --soft HEAD~1
- git reset --hard HEAD~1
- git reset --mixed HEAD~1
- git log --oneline #see git commit head


## Git Reset Cache

- git rm -r --cached directoryOrFileName


## Git Create branch

- git checkout -b newBranchName


## Git Delete Branch

- git branch -d localBranchName

- git push origin --delete remoteBranchName

- git push origin :fix/authentication

Use -D instead if you want to force the branch to be deleted, even if it hasn't been pushed or merged yet.

## Git History / Diff


## Git Unstash

## Git Rollback


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
- git checkout .


## Git Delete Branch

- git branch -d localBranchName

- git push origin --delete "remote branch name"

- git push origin :fix/authentication

You can use -D instead to force the branch to be deleted, even if it hasn't been pushed or merged yet.

## Git History / Diff


## Git Stash / UnStash
- git stash
- git stash pop #to apply the last stash
- git stash apply --index #to stash specific index
- git stash list #to list your stashed changes.
- git stash show #to see what n is in the below commands.
- git stash apply #to apply the most recent stash.
- git stash apply stash@{n} #to apply an older stash.

## Git Rollback
- git reset --hard HEAD@{"10 minutes ago"}

## Manage Multiple Repository from same code base
git remote add secondary https://github.com/user/repo2.git
git push secondary main
git pull secondary main
git pull origin main
git push origin main

## GPG Signed Push
gpg --version
gpg --list-secret-keys --keyid-format=long
gpg --full-generate-key //Generate new key
gpg --armor --export <your_key_id> // Export gpg key and add to github
git config --global user.signingkey <your_key_id> //attache signed key for repo
git config --global commit.gpgsign false //Disable gpg sign
git config --local commit.gpgsign false //disable repo base

### Run and kill gpg agent
gpgconf --kill gpg-agent
gpgconf --launch gpg-agent







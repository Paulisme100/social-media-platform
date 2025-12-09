# social-media-platform

if more people are working on the same branch always do
    git pull --rebase
before 
    git push
to load any commits from the remote branch (if it is ahead of your local branch)

if this results in a merge conflict 
you can manually solve the conflict, then
    git add <files with resolved conflicts>
after this, tell git that conflicts are solved so it can continue the rebase&merge (because the rebase was paused when conflict was spotted)
    git rebase --continue
if you didn't manage to solve the conflicts abort the rebase phase
    git rebase --abort

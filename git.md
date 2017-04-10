# Git
## Stash
   | git stash -u                        | Stash even unstaged files         |
   | git stash list                      | List all the available stashed    |
   | git stash show <id>                 | Show stash                        |
   | git stash show -p                   | Show most recent stash incl. diff |
   | git stash drop <stash>              | Delete stash                      |
   | git stash save <name>               | Save stash with name              |
   | git stash apply/pop stash^{/<name>} | Address stash with regex          |
   | git stash diff stash@{0}            | Diff the changes in the stash     |
   | git stash branch <branch> <stash>   | Create a branch from a stash      |
   |                                     |                                   |
## Branches
   | git checkout <branch>                                         | Switch to branch                                           |
   | git co <branch>                                               | Switch to branch                                           |
   | git branch <branch name>                                      | Add branch                                                 |
   | git checkout -b <branch>                                      | Create and switch to branch                                |
   | git push -u origin <branch>                                   | Push branch to remote and track                            |
   | git branch -vv                                                | Show verbose of verbose                                    |
   | git branch -d <branch>                                        | Delete local branch                                        |
   | git push origin --delete <branch>                             | Delete remote branch                                       |
   | git push origin <branch>                                      | Push commits to remote branch                              |
   | git checkout -b <local branch> origin/<name of remote branch> | Checkout remote branch                                     |
   | git merge --no-ff                                             | Merge with no fast-forward (ability to add info to commit) |
   | git diff <branch> <branch>                                    | See difference between branches                            |
   |                                                               |                                                            |
## Misc
   | git reset <file>                                        | Remove file from stage                                     |
   | git checkout [--] <file>                                | Revert file to original                                    |
   | git reset --hard HEAD                                   | Revert all changes                                         |
   | git unstage                                             | Unstage files                                              |
   | git reset HEAD --                                       | Unstage files                                              |
   | git clean -f -d                                         | Clean dir of untracked files and dirs                      |
   | git mergetool                                           | External merge tool                                        |
   | git remote                                              | Show remotes                                               |
   | git remote -v                                           | Show remotes verbose                                       |
   | git remote add origin <url>                             | Add an origin of <url> for origin                          |
   | git remote set-url origin <url>                         | Change remote url                                          |
   | git show --pretty="" --name-only <commit>               | Show filenames in commit                                   |
   | git fetch --all & git reset --hard oigin/<branch name>  | Force the pull to overwrite local files                    |
   |                                                         |                                                            |
## Log
   | git log -n <num>             | Show <num> number of logs messages              |
   | git show --stat <hash>       | Show the changed files for commit hash          |
   | git show <hash>              | Show the changes for commit hash                |
   | git diff <hash> <file>       | Show diff for file at commit hash               |
   | git log --decorate --numstat | Show files that were changed with log           |
   | git ls                       | Show log oneline with authors                   |
   | git ls --author=<author>     | Show log online of specific author              |
   | git ll                       | Show files that were changed with log           |
   | git lds                      | Show log showing dates                          |
   | git ld                       | Show log showing relative dates                 |
   | git log -u                   | Show commits and diff of file                   |
   | git st                       | Shorter status                                  |
   | git diff HEAD <file>         | Show changes in unstaged file                   |
   | git log <file>               | Show commits for <file>                         |
   | git log -p <file>            | Show commits with diffs for <file>              |
   | git shortlog -s -n           | Show summary of authors and their commits       |
   | git log --stat               | Show log with graph of added and removed things |
   | git log -p                   | Show log with diff                              |
   |                              |                                                 |
## Checkout
   | git reset --hard <hash/branch/tag> | Reset to hash, branch or tag        |
   | git checkout <hash/branch>         | Checkout/rollback to hash or branch |
   |                                    |                                     |
## Remotes
   | git push -u origin <branch> | Push branch to remote with tracking |
   |                             |                                     |
## Commit
   | git commit -am "message" | Add and commit with message                               |
   | git commit -a            | Add and commit                                            |
   | git reset --hard HEAD^   | Undo last commit and destroy those awful changes you made |
   | git reset --soft HEAD^   | Undo last commit and bring changes back into staging      |
   | git commit -v            | Show diff while writing message                           |
   |                          |                                                           |
## Tags
   | git tag                            | Show tags in repo       |
   | git push --tags origin HEAD:master | Push including tag info |
   |                                    |                         |
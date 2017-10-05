# Git

## Stash
| Command                                        | Description                                           |
|------------------------------------------------|-------------------------------------------------------|
| git stash                                      | Stash working copy                                    |
| git stash pop                                  | Pop most recent stash                                 |
| git stash drop                                 | Drop most recent stash                                |
| git stash -u                                   | Stash even unstaged files                             |
| git stash list                                 | List all the available stashes                        |
| git stash show `<id>`                          | Show stash                                            |
| git stash show -p                              | Show most recent stash incl. diff                     |
| git stash drop `<stash>`                       | Delete stash                                          |
| git stash save `<name>`                        | Save stash with name                                  |
| git stash apply/pop stash^{/`<name>`}          | Address stash with regex                              |
| git stash diff stash@{0}                       | Diff the changes in the stash                         |
| git stash branch `<branch>` `<stash>`          | Create a branch from a stash                          |
| git stash -p                                   | Enter into interactive mode and choose hunks to stash |
| git show `<stash>`:`<filename>`                | Show file in stash                                    |
| git show `<stash>`:`<filename>` > `<filename>` | Manually pull the file out from the stash             |
|||

## Branches
| Command                                                           | Description                                                       |
|-------------------------------------------------------------------|-------------------------------------------------------------------|
| git checkout `<branch>`                                           | Switch to branch                                                  |
| git co `<branch>`                                                 | Switch to branch                                                  |
| git branch `<branch name>` [`<branch>`/`<commit_hash>`/`<tag>`]   | Add branch                                                        |
| git checkout -b `<branch>`                                        | Create and switch to branch                                       |
| git push -u origin `<branch>`                                     | Push branch to remote and track                                   |
| git branch -vv                                                    | Show verbose of verbose (incl. tracking branches)                 |
| git branch -d `<branch>`                                          | Delete local branch                                               |
| git push origin --delete `<branch>`                               | Delete remote branch                                              |
| git push origin :`<remote_branch>`                                | Delete remote branch                                              |
| git push origin `<branch>`[:`<remote_branch_name>`]               | Push commits to remote branch                                     |
| git checkout -b `<local branch>` origin/`<name of remote branch>` | Checkout remote branch                                            |
| git merge --no-ff                                                 | Merge with no fast-forward                                        |
| git merge -e `<branch>`                                           | Merge with with ability to edit merge message                     |
| git merge --log[=`<n>`] `<branch>`                                | Merge with a shortlog of commits (max `<n>` commits) being merged |
| git diff `<branch>` `<branch>`                                    | See difference between branches                                   |
| git br                                                            | Show a list of all branches with their creation dates and authors |
| git branch --set-upstream `<branch>` `<remote>/<branch>`          | Set up tracking between local and remote branches                 |
| git branch -m `<branch_name>` `<branch_name>`                     | Rename branch                                                     |
| git branch `<branch_name>` `<hash>`                               | Create a branch from `<hash>` (can be done from reflog also)      |
|||

## Misc
| Command                                                    | Description                                                         |
|------------------------------------------------------------|---------------------------------------------------------------------|
| git reset `<file>`                                         | Remove file from stage                                              |
| git checkout [--] `<file>`                                 | Revert file to original (HEAD)                                      |
| git unstage                                                | Unstage files                                                       |
| git reset HEAD --                                          | Unstage files                                                       |
| git clean -n                                               | What would the clean command do                                     |
| git clean                                                  | Clean all files in working copy                                     |
| git clean -f -d                                            | Clean dir of untracked files and dirs                               |
| git mergetool                                              | External merge tool                                                 |
| git remote                                                 | Show remotes                                                        |
| git remote -v                                              | Show remotes verbose                                                |
| git remote add origin `<url>`                              | Add an origin of `<url>` for origin                                 |
| git remote set-url origin `<url>`                          | Change remote url                                                   |
| git remote rm origin                                       | Remove remote url                                                   |
| git remote prune <remote>                                  | Prune refs to branches that aren't there anymore                    |
| git show --pretty="" --name-only `<commit>`                | Show filenames in commit                                            |
| git fetch --all & git reset --hard origin/`<branch name>`  | Force the pull to overwrite local files                             |
| git fetch [`<remote>`]                                     | Fetch changes                                                       |
| git pull                                                   | Fetch changes and merge (git fetch && git merge `<remote>/<branch>` |
| git add -u                                                 | Add updated tracked files to stage                                  |
| git add -A                                                 | Add all tracked and untracked files to stage                        |
| git reflog                                                 | Show all references where HEAD has pointed to for last 30 days      |
| git cherry-pick `<hash>`                                   | Cherry pick hash into current branch                                |
|||

## Config
|------------------------------------------------------------|------------------------------------------------------------|
| git config --global -e                                     | Open global config for editing                             |
| git config -e                                              | Open local config for editing                              |
| git config --system -e                                     | Open system config for editing                             |
| git config --list                                          | List all options                                           |
|||

## Log
| Command                                        | Description                                      |
|------------------------------------------------|--------------------------------------------------|
| git log -n `<num>`                             | Show `<num>` number of logs messages             |
| git show --stat `<hash>`                       | Show the changed files for commit hash           |
| git show `<hash>`                              | Show the changes for commit hash                 |
| git diff `<hash>` `<file>`                     | Show diff for file at commit hash                |
| git diff `<hash>`..`<hash>`                    | Show diff between two hashes                     |
| git diff HEAD~1..HEAD                          | Show diff for one behind HEAD (HEAD~1) and HEAD  |
| git diff `<hash>`..                            | Show diff for hash and HEAD                      |
| git diff --cached [`<filename>`]               | Show diff for HEAD and stage                     |
| git log --decorate --numstat                   | Show files that were changed with log            |
| git ls                                         | Show log oneline with authors                    |
| git ls --author=`<author>`                     | Show log online of specific author               |
| git ll                                         | Show files that were changed with log            |
| git lds                                        | Show log showing dates                           |
| git ld                                         | Show log showing relative dates                  |
| git log -u                                     | Show commits and diff of file                    |
| git st                                         | Shorter status                                   |
| git diff HEAD `<file>`                         | Show changes in unstaged file                    |
| git log `<file>`                               | Show commits for `<file>`                        |
| git log -p `<revision>` `<file>`               | Show commits with diffs for `<file>` at revision |
| git shortlog -s -n -e                          | Show summary of authors and their commits        |
| git log --stat                                 | Show log with graph of added and removed things  |
| git log -p                                     | Show log with diff                               |
| git log --follow `<filename>`                  | List commits for `<filename>`                    |
| git log --all --full-history -- <path-to-file> | Show log for deleted file                        |
|                                                |                                                  |

## Checkout
| Command                                | Description                                                  |
|----------------------------------------|--------------------------------------------------------------|
| git reset --hard `<hash/branch/tag>`   | Reset to hash, branch or tag                                 |
| git reset --hard [HEAD]                | Revert all changes to HEAD                                   |
| git reset --soft HEAD~1                | Rollback/undo to last commit put files in working copy area  |
| git reset --hard HEAD~1                | Rollback/undo to last commit discard files from commit       |
| git checkout `<hash/branch>`           | Checkout/rollback to hash or branch                          |
| git co `<hash>` `<file_path_and_name>` | Checkout `<file>` from `<hash>`                              |
| git checkout tags/`<tag>`              | Checkout tag                                                 |
|                                        |                                                              |

## Remotes
| Command                       | Description                         |
|-------------------------------|-------------------------------------|
| git push -u origin `<branch>` | Push branch to remote with tracking |
|                               |                                     |

## Commit
| Command                  | Description                                               |
|--------------------------|-----------------------------------------------------------|
| git commit -am "message" | Add and commit with message                               |
| git commit -a            | Add and commit                                            |
| git reset --hard HEAD^   | Undo last commit and destroy those awful changes you made |
| git reset --soft HEAD^   | Undo last commit and bring changes back into staging      |
| git commit -v            | Show diff while writing message                           |
|                          |                                                           |

## Tags
| Command                            | Description             |
|------------------------------------|-------------------------|
| git tag                            | Show tags in repo       |
| git tag `<tag>`                    | Add tag                 |
| git tag -a `<tag>`                 | Add tag with message    |
| git push --tags                    | Push tag info           |
| git push --tags origin HEAD:master | Push including tag info |
|                                    |                         |

## Submodules
| Command                                                | Description                                        |
|--------------------------------------------------------|----------------------------------------------------|
| git submodule                                          | List all submodules                                |
| git submodule update [--init --recursive]              | Pull down all submodules                           |
| git submodule add `<submodule_url>` `<submodule_name>` | Add submodule to repo                              |
| git clone --recursive `<project_url>`                  | Clone repo including submodules and their contents |
|||



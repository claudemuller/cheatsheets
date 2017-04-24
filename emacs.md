# Emacs

## Engine Mode
| Command | Description         |
|---------|---------------------|
| C-c / g | Search Google       |
| C-c / d | Search Duck Duck Go |
|||

## General
| Command                        | Description                                              |
|--------------------------------|----------------------------------------------------------|
| C-x C-c                        | End emacs session                                        |
| C-x C-o                        | Other window                                             |
| C-v                            | Next page/screen                                         |
| M-v                            | Previous page/screen                                     |
| C-l                            | Move screen to middle -> top -> bottom                   |
| C-u 0 C-l                      | Move screen+point to top                                 |
| C-/                            | Undo                                                     |
| C-x 1                          | Kill all other windows (keep this 1)                     |
| C-d                            | Delete character before point                            |
| M-d                            | Delete word after point                                  |
| C-SPC                          | Start selection/mark                                     |
| C-x C-r                        | Open file as root                                        |
| C-x C-f                        | Find file                                                |
| C-x C-s                        | Save file                                                |
| C-x b                          | List buffers                                             |
| C-c b                          | Switch to other buffer                                   |
| C-x s                          | Save some buffers                                        |
| C-z                            | Suspend/minimise emacs                                   |
| C-x f                          | Set margin                                               |
| M-q                            | Refill paragraph                                         |
| C-s                            | Search forward                                           |
| C-r                            | Reverse search                                           |
| C-x 2                          | Split window horizontally                                |
| C-x 3                          | Split window vertically                                  |
| C-M-v                          | Scroll other window down                                 |
| C-M-S-v                        | Scroll other window up                                   |
| C-x 4 f                        | Open file in vertically split window                     |
| C-x 5 f                        | Open file in new frame                                   |
| C-x 4 b                        | Buffer in new window                                     |
| C-x 5 b                        | Buffer in new frame                                      |
| C-x k                          | Kill buffer                                              |
| C-x 0                          | Kill this window                                         |
| ESC ESC ESC                    | Exit recursive editing level                             |
| M-;                            | Comment/uncomment                                        |
| C-x C-w                        | Save to new filename                                     |
| C-u C-SPC                      | Move point back to previous position                     |
| C-M-n                          | Jump forward parenthesis                                 |
| C-M-p                          | Jump backward parenthesis                                |
| C-S-c C-S-c                    | Turn selection into multiple cursors                     |
| C->                            | Mark next instance of selected word for multiple cursors |
| C-<                            | Unmark instance of selected word for multiple cursors    |
| M-O                            | Insert a line above the current line                     |
| M-o                            | Insert a line below the current line                     |
| C-M-\                          | Reindent all the lines in the region                     |
| C-M-q                          | Reindent                                                 |
| C-M->                          | Move selection right by one character                    |
| C-M-<                          | Move selection left by one character                     |
| C-S-p                          | Start selection/mark and move up one line                |
| C-S-n                          | Start selection/mark and move down one line              |
| C-S-M-p                        | Start selection/mark and move up one paragraph           |
| C-S-M-n                        | Start selection/mark and move down one line              |
| M-}                            | Move to next paragraph                                   |
| M-{                            | Move to previous paragraph                               |
| C-M-p                          | Jump to opening bracket                                  |
| C-M-n                          | Jump to closing bracket                                  |
| M-x kill-some-buffers          | Prompt before killing each buffer                        |
| M-!                            | Shell command                                            |
| M-&                            | Asynchronous shell command                               |
| C-u M-!/M-&                    | Shell output in current buffer                           |
| M-x ansi-term                  | Terminal                                                 |
| C-x 5 2                        | Create new frame                                         |
| C-x 5 0                        | Kill current frame                                       |
| C-S-up/down/left/right         | Resize window                                            |
| M-z `<val>`                    | Delete up to `<val>`                                     |
| M-x surround                   | Surround text with opening and closing text              |
| S-`<arrow>`                    | Switch to other window                                   |
| C-x (                          | Start recording macro                                    |
| C-x )                          | Stop recording macro                                     |
| C-x e                          | Run last macro                                           |
| M-l                            | Convert following word to lower case (downcase-word).    |
| M-u                            | Convert following word to upper case (upcase-word).      |
| M-c                            | Capitalize the following word (capitalize-word).         |
| C-x C-l                        | Convert region to lower case (downcase-region).          |
| C-x C-u                        | Convert region to upper case (upcase-region).            |
| M-x shell-command-on-region    | Execute shell command on region                          |
| M-%                            | Find and replace                                         |
| C-=                            | Select region by semantic units                          |
| M-.                            | Jump to tag                                              |
| M-*                            | Pop back to previous position after M-.                  |
| M-x kill-compilation           | Kill current running (compile) sub-process               |
| M-x fci-mode                   | Show fill column indicator                               |
| C-x f                          | Set fill column indicator                                |
| M-x toggle-truncate-lines      | Toggle truncate long lines                               |
| M-x json-reformat-region       | Reflow/indent .json                                      |
| M-x projectile-cleanup-known-projects | Clear cache of invalid projects                          |
| C-c I                          | PHP online documentation                                 |
|                                |                                                          |

## Bookmarks
| Command                        | Description      |
|--------------------------------|------------------|
| C-x r m                        | set bookmark     |
| C-x r b                        | jump to bookmark |
| C-x r l                        | list bookmarks   |
|||

## Copy/Kill/Yank
| Command                        | Description                    |
|--------------------------------|--------------------------------|
| C-w                            | Kill selection                 |
| C-y                            | Yank selection back            |
| M-y                            | Cycle through previous kills   |
| C-k                            | Kill from point to end of line |
| M-w                            | Copy to kill ring              |
|||

## Movement
| Command                        | Description                                    |
|--------------------------------|------------------------------------------------|
| C-p                            | Up one line                                    |
| C-n                            | Down one line                                  |
| C-b                            | Back one character                             |
| C-f                            | Forward one character                          |
| M-r                            | Move point to middle -> top -> bottom          |
| C-u 0 M-r                      | Move point to beginning of screen              |
| M-f                            | Move forward by one word                       |
| M-b                            | Move backward by one word                      |
| C-a                            | Move to beginning of line                      |
| C-e                            | Move to end of line                            |
| M-a                            | Move to beginning of sentence                  |
| M-e                            | Move to end of sentence                        |
| M-<                            | Move to beginning of text                      |
| M->                            | Move to end of text                            |
| C-u `<num>`                    | Repeat `<num>` times                           |
| M-m                            | Move point to beginning of code (after indent) |
| M-g g                          | Go to line number                              |
|||

## Help
| Command                        | Description                              |
|--------------------------------|------------------------------------------|
| C-h c                          | Help with command                        |
| C-h k                          | Help with key sequence                   |
| C-h f                          | Help with function                       |
| C-h v                          | Help with variable                       |
| C-h a                          | Command apropos (search help by keyword) |
|||

## Dired Mode
| Command                           | Description                                            |
|-----------------------------------|--------------------------------------------------------|
| C-x d                             | Dired mode                                             |
| Q                                 | Find and replace regex in marked files                 |
| R                                 | Rename file                                            |
| D                                 | Delete file                                            |
| x                                 | Delete files/directories that were marked for deletion |
| C                                 | Copy file to directory or to new name                  |
| +                                 | Create a directory                                     |
| m                                 | Mark files                                             |
| u                                 | Remove mark from                                       |
| * s                               | Mark all files in current sub directory                |
| U                                 | Unmark all marked files and directories                |
| M-x find-name-dired               | Search for files by pattern including sub directories  |
| g                                 | Update buffer                                          |
| M-x find-dired                    | Run find in directory                                  |
| s                                 | Toggle between alphabetical and date order             |
| M-x grep -nH -e "term" ./**/*.ext | Grep in this and child dirs by term in .ext            |
|                                   | -n show line numbers; -H show filenames; -e expression |
|                                   |                                                        |

## Emmet Mode
| Command                        | Description    |
| C-j                            | Expand snippet |
|||

## Helm/Projectile Mode
| Command                        | Description                     |
|--------------------------------|---------------------------------|
| C-c p p                        | Change project                  |
| C-c p f                        | Find file                       |
| C-c p h                        | Find mixed files/buffers/recent |
| C-c o                          | Open in new window split        |
| C-c C-o                        | Open in new frame               |
| C-c r                          | Open file as root               |
| \pp                            | Helm Projectile switch project  |
| \pf                            | Helm Projectile                 |
|||

## Magit Mode
| Command                        | Description       |
|--------------------------------|-------------------|
| C-c M                          | Magit-status      |
| s                              | Stage             |
| u                              | Unstage           |
| k                              | Discard/delete    |
| i                              | Ignore            |
| TAB                            | View diff of file |
| enter                          | Edit file         |
| c                              | Commit menu       |
| C-c C-c                        | Save the commit   |
| P                              | Push menu         |
| $                              | Status message    |
| F                              | Fetch menu        |
| l                              | Log menu          |
|||

## Neotree Mode
| Command                        | Description           |
|--------------------------------|-----------------------|
| C-c N                          | Toggle neotree mode   |
| C-c C-n                        | New file              |
| H                              | Toggle hidden files   |
| C-c C-c                        | Change root directory |
| C-c C-r                        | Rename file/directory |
| C-c C-d                        | Delete file/directory |
|||

## Org Mode
  - http://orgmode.org/orgcard.txt
    # -*- mode: org -*-
    #+STARTUP: overview/content/showall/showeverything
    #+TAGS: { @OFFICE(o) @HOME(h) } COMPUTER(c) PHONE(p) READING(r)

| Command                        | Description                                   |
|--------------------------------|-----------------------------------------------|
| M-RETURN                       | Start a new heading, bullet point etc.        |
| C-RETURN                       | Create new heading                            |
| M-RIGHT/LEFT                   | Promote/demote item                           |
| M-S-RIGHT/LEFT                 | Promote/demote item including sub items       |
| S-RIGHT/LEFT                   | Change list bullet type                       |
| M-UP/DOWN                      | Reorder list                                  |
| S-LEFT/RIGHT                   | Add/remove TODO/IN-PROGRESS etc.              |
| TAB                            | Expand/contact section                        |
| C-c C-c                        | Enter tags when done on heading               |
| C-c C-t                        | Toggle todo                                   |
| C-c +                          |                                               |
| C-c C-d                        | Create deadline                               |
| C-c C-n                        | Jump to next heading                          |
| C-c C-p                        | Jump to previous heading                      |
| C-c C-f                        | Jump to next heading of same level            |
| C-c C-b                        | Jump to previous heading of same level        |
| C-c C-d                        | Set deadline                                  |
| S-TAB                          | Cycle through different levels of indentation |
| C-c [                          | Add file to front of agenda                   |
| C-c ]                          | Remove file from agenda                       |
| C-x n w                        | Widen buffer to whole tree                    |
| C-x n s                        | Narrow buffer to current subtree              |
| C-c C-o                        | Open link                                     |
| C-c l                          | Create an Org link to current file and pos    |
| C-c C-l                        | Paste/insert a recorded Org link              |
|                                | With cursor on link -> edit Org link          |
| C-c c                          | Invoke Org-capture                            |
| C-c s                          | With point on parent TODO, sort children      |
| C-c .                          | Add date                                      |
| C-u C-c .                      | Add a date and time                           |
| C-c C-s                        | Schedule date                                 |
| C-c C-e                        | Export                                        |
| C-c C-x C-a                    | Archive subtree                               |
| M-x toggle-truncate-lines      | Toggle line wrap                              |
| \sl                            | Org store link                                |
| \ol                            | Org open link                                 |
|||

## In table
 | Command                        | Description           |
 |--------------------------------|-----------------------|
 | M-S-LEFT/RIGHT                 | Add/remove column     |
 | M-S-UP/DOWN                    | Add/remove row        |
 | C-c C-c                        | Redraw table on table |
 |||

 ## Checkboxes
| Command         |                 |
|-----------------|-----------------|
| use [/] and [%] | With checkboxes |
| C-c C-c         | Tick checkbox   |
|||

## Yasnippet Mode
| Command                        | Description          |
|--------------------------------|----------------------|
| M-x yas-new-snippet            | Create a new snippet |
| C-c Y                          | Complete snippet     |
|                                |                      |

## Web Mode
| Command                        | Description                                  |
|--------------------------------|----------------------------------------------|
| C-c C-d                        | Delete inside tag                            |
| C-c C-e r                      | Change tag name                              |
| C-c I                          | Load PHP docs for function/variable at point |
| web-mode-set-engine            | Set Web mode engine                          |
|                                |                                              |





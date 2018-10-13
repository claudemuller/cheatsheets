# Vim

## Movement
| Command  | Description                                 |
|----------|---------------------------------------------|
| j        | Down 1 line                                 |
| k        | Up 1 line                                   |
| h        | Left 1 character                            |
| l        | Right 1 character                           |
| f        | Find next occurance                         |
| F        | Find previous occurance                     |
| t        | Find next occurance stop before find        |
| T        | Find previous occurance stop before find    |
| .        | Repeat f/t                                  |
| H        | High - move cursor to top of window         |
| M        | Middle - move cursor to middle of window    |
| L        | Low - move cursor to bottom of window       |
| w        | Jump beginning of word                      |
| e        | Jump end of word                            |
| b        | Jump to beginning of previous word          |
| ge       | Jump to end of previous word                |
| zz       | Center screen where cursor is               |
| zt       | Move screen to top of screen                |
| zb       | Move screen to bottom of screen             |
| ^        | Beginning of text on line                   |
| 0        | Beginning of line                           |
| $        | End of line                                 |
| G        | Jump to end of file                         |
| gg       | Jump to beginning of file                   |
| %        | Matching parenthesis                        |
| `<num>`G | Jump to `<num>` line number                 |
| Ctrl-D   | Move half-page down                         |
| Ctrl-U   | Move half-page up                           |
| Ctrl-B   | Page up                                     |
| Ctrl-F   | Page down                                   |
| Ctrl-O   | Jump to last (older) cursor position        |
| Ctrl-I   | Jump to next cursor position (after Ctrl-O) |
|          |                                             |

## Viewing Code
| Command                   | Description                                  |
|---------------------------|----------------------------------------------|
| #                         | Select all occurances of string under cursor |
| :set foldmethod=indent    | Set indent style to indent                   |
| :set foldmethod=syntax    | Set indent style to syntax                   |
| za                        | Toggle fold                                  |
| zo                        | Open fold                                    |
| zc                        | Close fold                                   |
| zA                        | Toggle fold recursively                      |
| zO                        | Open fold recursively                        |
| zC                        | Close fold recursively                       |
| m<letter>                 | Set mark                                     |
| '<letter>                 | Go to mark                                   |
|                           |                                              |

## Deletion
| Command | Description                      |
|---------|----------------------------------|
| x       | Delete character at point        |
| dd      | Delete line                      |
| dw      | Delete word                      |
| db      | Delete word backwards            |
| d^      | Delete to beginning of line      |
| d$      | Delete to end of line            |
| diw     | Delete inner word                |
| D       | Delete from point to end of line |
| ds"     | Delete delimeters                |
| dst     | Delete tag                       |
|         |                                  |

## Editing
| Command               | Description                            |
|-----------------------|----------------------------------------|
| i                     | Insert at point                        |
| I                     | Insert at beginning of line            |
| a                     | Append at point                        |
| A                     | Append at end of line                  |
| R                     | Replace mode                           |
| r                     | Replace                                |
| c                     | Change                                 |
| ce                    | Change to end of word                  |
| ciw                   | Change inner word                      |
| :s/find/replace/g     | Find & replace                         |
| :1,20s/find/replace/g | Find & replace between line 1,20       |
| :%s/find/replace/g    | Find & replace in whole buffer         |
| J                     | Join lines                             |
| o                     | New line below point                   |
| O                     | New line above point                   |
| y                     | Yank/copy selection                    |
| p                     | Paste                                  |
| " * y			| Yank to system clipboard 		 |
| " * p			| Paste to system clipboard 		 |
| ~                     | Upper/lowercase character              |
| >                     | Indent of code                         |
| cs"'                  | Inside "" change to ''                 |
| cs'`<p>`              | Change ' to `</p>`                     |
| cst"                  | Change tag to "                        |
| cs"                   | Change delimeters                      |
| cst                   | Change tag                             |
| ca"                   | Change including outer "               |
| ysiw[                 | Surround inner word with [             |
| S`<p>`                | Surround selection with `</p>`         |
| yssm[                 | Surround whole line in [               |
| cc                    | Clear line and start at indent         |
| C                     | Clear from point and enter insert mode |
| gg=G                  | Reindent code                          |
| =%                    | Reindent this block of code            |
| :norm i#              | Insert #'s at the beginning of line(s) |
|                       |                                        |

## Windows & Tabs
| Command        | Description                          |
|----------------|--------------------------------------|
| Ctrl-w h/j/k/l | Jump to window at left/down/up/right |
| Ctrl-w H/J/K/L | Move window around                   |
| gt             | Next tab                             |
| gT             | Previous tab                         |
| [num]gt        | Jump to [num] tab                    |
|                |                                      |

## Search
| Command        | Description                         |
|----------------|-------------------------------------|
| /              | Search                              |
| ?              | Search backwards                    |
| n              | Next occurance of search result     |
| N              | Previous occurance of search result |
| /\c<term>      | Search case insensitive             |
| /\C<term>      | Search case sensitive               |
|||

## General
| Command     | Description           |
|-------------|-----------------------|
| u           | Undo last commands    |
| U           | Fix whole line        |
| :w          | Save                  |
| :wq         | Save & quit           |
| Shft + zz   | Save & quit           |
| :!          | Execute shell command |
| v           | Select                |
| :r filename | Retrieve filename     |
|             |                       |

## Registers
| Command     | Description                                                         |
|-------------|---------------------------------------------------------------------|
| "ayy        | Yank current line and put it in register 'a'                        |
| "Ayy        | Append to a register - yank current line and append to register 'a' |
| "ap         | Paste the contents of register 'a'                                  |
| "+p         | Paste from the system clipboard in Linux                            |
| "*p         | Paste form the system clipboard in Windows                          |
| :reg        | Access all currently defined registers                              |
|             |                                                                     |

## Leader Keys
| Command     | Description                    |
|-------------|--------------------------------|
| \c          | Org capture                    |
| \sl         | Org store link                 |
| \ol         | Org open link                  |
| \k          | Kill buffer                    |
| \f          | Open file                      |
| \b          | Open buffer                    |
| \pp         | Helm Projectile switch project |
| \pf         | Helm Projectile                |
|             |                                |


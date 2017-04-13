# Pacman

## General
| Command                        | Description                                                                                                                                             |
|--------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------|
| pacman -Qs string1 string2 ... | To search for already installed packages                                                                                                                |
| pacman -Si package_name        | To display extensive information about a given package                                                                                                  |
| pacman -Qi package_name        | For locally installed packages                                                                                                                          |
| pacman -Qii package_name       | Passing two -i flags will also display the list of backup files and their modification states                                                           |
| pacman -Ql package_name        | To retrieve a list of the files installed by a package                                                                                                  |
| pacman -Qk package_name        | verify the presence of the files installed by a package:                                                                                                |
| pacman -Qo /path/to/file_name  | Passing the k flag twice will perform a more thorough check. One can also query the database to know which package a file in the file system belongs to |
| pacman -Qdt                    | To list all packages no longer required as dependencies (orphans)                                                                                       |
| pacman -Qet                    | To list all packages explicitly installed and not required as dependencies                                                                              |
| pacman -Rdd                    | Remove only this package                                                                                                                                |
|                                |                                                                                                                                                         |


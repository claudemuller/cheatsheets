# Python cheatsheet

- Multi-line string

``` python
var = ''' This is
a multi-line string'''
```

- Format a string

``` python
print("%s %s" % ("one", "two"))
```

## Lists
  list.append(val)
  list.insert(location, val)
  list.remove(val)
  list.sort()
  list.reverse()
  del list[1]
  len(list)

## File operations
  # open file for (r)ead or (w)rite
  f = open.('filename.txt', 'r')  # 'w'

  # read entire file
  data = f.read()
  # or line by line
  for line in f:
      # do some magic

  # write to file
  f.write('something here')

  # close file
  f.close()

## VirtualEnv
  cd the_project_in_question
  virtualenv env_name
  # virtualenv -p /usr/bin/python2.7 env_name     # for python version specific
  source env_name/bin/activate                    # activate virtualenv
  deactivate                                      # deactivate virtualenv

  pip freeze > requirements.txt                   # save a list of requirements
  pip install -r requirements.txt                 # install from list

## Tuples
- Tuples do NOT need surrounding ()'s

*Tuple assignment*

``` python
  a, b = 3, 1
```

- Gather parameter - multiple arguments

``` python
def a_function(*args):
    pass

a_function(1, 2, 3)
```

- Scatter parameter - scatter tuple into multiple parameters

``` python
t = (1, 2)
a_function(*t)
```

## Tkinter
  - Tkinter → tkinter
  - tkMessageBox → tkinter.messagebox
  - tkColorChooser → tkinter.colorchooser
  - tkFileDialog → tkinter.filedialog
  - tkCommonDialog → tkinter.commondialog
  - tkSimpleDialog → tkinter.simpledialog
  - tkFont → tkinter.font
  - Tkdnd → tkinter.dnd
  - ScrolledText → tkinter.scrolledtext
  - Tix → tkinter.tix
  - ttk → tkinter.ttk

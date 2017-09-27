# Core: Unix Utilities

_More powerful than the spiky blue shell_

## Challenges, Part 1

Challenges within each section are meant to be solved in order.

### Navigation

1.  Print the path of your working directory
    - `pwd`
1.  List the files in your working directory
    - `ls`
1.  List the files with a particular extension, like `.txt`
    - `ls **/*.txt`
1.  List the files in a subdirectory, like `project`
    - `ls ./project`
1.  Navigate to a subdirectory, like `project`
    - `cd project`
1.  Navigate to the parent directory of your working directory
    - `cd ..`
1.  Navigate to a nested subdirectory, like `path/to/project`
    - `cd path/to/project`
1.  Navigate to your home directory
    - `cd`
1.  Navigate back to the previous directory
    - `cd -`

### Variables

1.  Print a sentence, like `Hello world`
    - `print Hello \World`
1.  Print a variable value, like `$USER` or `$PATH`
    - `print $USER` or `print $PATH`
1.  Set a variable `NAME` equal to your first name, then print its value
    - `NAME=Willie` then `print $NAME`
1.  Set a variable `FULL_NAME` equal to your full name, then print its value
    - `FULL_NAME="Willie Johnson"`
1.  Print all environment variables (names and values)
    - `printenv`
1.  Make an alias named `hello` that prints `Hello world`
    - `alias hello="print Hello \World"`
1.  Make an alias named `gocode` that navigates to your code directory
    - `alias gocode="~\Documents\GitHub"`
1.  Print all aliases (names and values)
    - `alias`

### Getting Help

1.  Print what options a command accepts, like `bash` or `python`
1.  Read the manual for a command, like `echo` or `ls`
1.  Print the file path to a command, like `bash` or `python`

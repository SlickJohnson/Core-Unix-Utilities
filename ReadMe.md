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
    - `bash` then press *tab* twice
1.  Read the manual for a command, like `echo` or `ls`
    - `man echo` or `man ls`
1.  Print the file path to a command, like `bash` or `python`
    - `echo "$PWD/bash"` or `echo "$PWD/python"`

### Files

1.  Navigate to the directory `Animals`
    - `cd Animals`
1.  Print the contents of the file `Cats.txt`
    - `cat Cats.txt`
1.  Print the contents of both files `Cats.txt` and `Dogs.txt`
    - `cat Cats.txt; cat Dogs.txt`
1.  Count the words in the file `Cats.txt`
    - `wc -l Cats.txt`
1.  Count the words in all files with the extension `.txt`
    - `wc -l *.txt`
1.  Copy the file `Dogs.txt` to a new file `BabyDogs.txt`
    - `cp Dogs.txt BabyDogs.txt`
1.  Rename the file `BabyDogs.txt` to `Puppies.txt`
    - `mv BabyDogs.txt Puppies.txt`
1.  Make a new directory named `Shelter` inside `Animals`
    - `mkdir Shelter`
1.  Move the file `Puppies.txt` into the directory `Shelter`
    - `mv Puppies.txt ./Shelter/`
1.  Copy the file `Cats.txt` to `Kittens.txt` inside `Shelter`
    - `cp Cats.txt ./Shelter/Kittens.txt`
1.  List the files within the directory `Shelter`
    - `ls Shelter/`
1.  Count the words in all `.txt` files inside `Shelter`
    - `wc -w /Shelter/*.txt`
1.  Try to remove the directory `Shelter` (this should fail)
    - `rm Shelter`
1.  Remove all `.txt` files inside `Shelter`
    - `rm ./Shelter/*.txt`
1.  Remove the directory `Shelter` (this should succeed)
    - `rm Shelter`
1.  Now cry because you just deleted those poor tiny animals
    - `Cry`

### Permissions

1.  Print out your user name
    - `print $USER`
1.  List the permissions (and metadata) of all `.txt` files
    - `ls -l ./**/*.txt`
1.  Give all users write permission on the file `Cats.txt`
    - `chmod a+r+w Cats.txt`
1.  List the permissions (and metadata) of the file `Cats.txt`
    - `ls -l Cats.txt`
1.  Change the owner of the file `Cats.txt` to another user
    - `sudo chown nobody Cats.txt`
1.  Now list the permissions (and owner) of the file `Cats.txt`
1.  Try to change the owner of the file `Cats.txt` back to yourself
    - `chown $USER Cats.txt`
1.  Invoke the super-user to make the previous command succeed
    - `sudo chown nobody Cats.txt`
1.  List the permissions (and owner) of the file `Cats.txt` again
    - `ls -l Cats.txt`

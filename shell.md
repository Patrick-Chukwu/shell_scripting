

# Table of Contents 
- [Intro to Shell](#shell)
- [Navigation](#navigation)
- [Manipulating Files](#files)
    - [Wildcards](#wildcards)
- [Working with Commands](#commands)
- [I/O Redirection](#ioredirection)
- [Expansion](#expansion)
- [Permissions](#permissions)
- [Job Control](#jobcrontrol)

## Shell
Shell is a program that takes commands from the keyboard and gives them to the operating system to perform. On most Linux systems, **bash** (*Bourne Again Shell*) acts as the shell program. Other available shells include: **ksh**, **tcsh**, **zsh**.

- **GUI**: *Graphical User Interface*
- **CLI**: *Command Line Interface*

### What is a "Terminal?"
It's a program called a ***terminal emulator***. It simply opens a window and lets you interact with the shell.

## Navigation
To navigate your system files and directories (folders), you need to be used to a few commands. They are discussed below:
- **pwd**: Print Working Directory
- **cd**: change directory
- **ls**: List files/directories
- **less**: view text files
- **file**: classify a file's content. e.g `file name_of_file`


##### Commands are generally in this form:
***command -options arguments***, e.g: `ls -la ..`

##### COntrolling less
- Page Up or b - Scroll back
- Page Down or space - Scroll forward
- G - Go to the end of the text file
- 1G - Go to the beginning of the text file
- /characters - Search forward in the text file 
- n - Repeat previous search
- h - help
- q - quit

## Files
- **cp** - copy files and directories
- **mv** - move or rename files and directories
- **rm** - create directories
- **mkdir** - create directories

### Wildcards
Wildcards are special characters that helps rapidly specify groups of filenames. It allows you select filenames based on patterns of characters.

#### Types of wildcards
- * - Matches any characters
- ? - Matches any single character
- [characters] - Matches any character that is a member of the set characters. It can also be expressed as a ***POSIX character class***, such as **[:alnum:]** - alphanumeric, **[:alpha:]** - alphabetic, **[:digit:]** - numeric, **[:upper:]** - Uppercase alphabetic & **[:lower:]** - lowercase alphabetic characters.
- [!characters] - Matches any character that is not a member of the set of characters.

### Examples of wildcards
- * - All filenames
- g* - ll filenames that begins with g
- b*.txt - All filenames that begins with b and ends i  .txt
- Data??? - Any filename that begin with character "Data" and followed  by exactly 3 more characters.
- [abc]* - Any filename that begins with either "a", "b", "c" and followed by any other characters.
- 

#### popular options with the above file manipulation commands
- ***-i*** - interactive: the user is prompted before the action
- ***-R*** - forced: it creates the file/directory if it doesn't exist.
- ***-r*** - recursion : Used along `rm` to delete directories alongside all the contents inside.

## Commands
Commands can be one of four different kinds:
1. *An executable program*. Programs can be compiled binaries written in C and C++ pr in scripting languages like shell, Perl, Python, Ruby etc.
2. *A command built into the shell itself* : Bash provides  a number of commands internally called shell builtins. e.g `cd`
3. *A shell function* : These are miniature shell scripts incorporated into the environment.
4. *An alias*: Commands that we can define ourselves built from other commands.

### Identifying commands 
- **type** - Display information about command type : `type command`
- **which** - Locate a command : `which command`
- **help** - Display reference page for shell builtin `help command` or `command --help`
- **man** - Display an on-line command reference `man command`

## I/O Redirection
We can redirect the output of commands to files, devices and even to the input of other commands.


### Standard output

- ***>*** We use `>` to redirect the output of a command to a file
- ***<*** We use `<` to redirect the input to a command into a file

### Pipelines
Pipelines help connect multiple commands together
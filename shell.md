

# Table of Contents 
- [Intro to Shell](#shell)
- [Navigation](#navigation)
- [Manipulating Files](#files)
    - [Wildcards](#wildcards)


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
- /* - Matches any characters
- ? - Matches any single character
- [characters] - Matches any character that is a member of the set characters. It can also be expressed as a ***POSIX character class***, such as **[:alnum:]** - alphanumeric, **[:alpha:]** - alphabetic, **[:digit:]** - numeric, **[:upper:]** - Uppercase alphabetic & **[:lower:]** - lowercase alphabetic characters.
- [!characters] - Matches any character that is not a member of the set of characters.

### Examples of wildcards

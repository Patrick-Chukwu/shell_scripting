

# Table of Contents 
- [Intro to Shell](#shell)
- [Navigation](#navigation)


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
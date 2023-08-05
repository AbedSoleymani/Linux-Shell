# Linux-Shell

A **terminal**, also known as a **command-line interface (CLI)**, **shell**, or **console**, is a text-based interface used to interact with a computer's operating system and execute commands. It provides a way to communicate with the computer using text commands rather than a graphical user interface (GUI).

In a terminal, you can enter commands and receive text-based responses from the computer. This allows you to perform various tasks, such as navigating the file system, running programs, managing files and directories, configuring system settings, and more. Terminals are commonly used in programming, system administration, and various technical tasks.

## The Terminal vs. The Shell
"Terminal" and "shell" are related concepts in the context of command-line interfaces, but they refer to different components. Let's clarify the difference between the two:

* **Terminal:**<br>
A terminal is a software application that provides a user interface to interact with the command-line environment of an operating system.<br>
It is often referred to as a "terminal emulator" because it emulates a physical terminal (text-based input and output device) within a graphical user interface.<br>
The terminal provides a window where you can type commands and see their output.<br>
It handles the rendering of text and the communication between the user and the shell.<br>
Examples of terminal programs include GNOME Terminal, iTerm2, Command Prompt, and Windows Terminal.<br>
* **Shell:** <br>
A shell is a command-line interpreter that provides a command-line interface for interacting with the operating system.<br>
It is a program that takes the commands you enter and executes them by communicating with the operating system kernel.<br>
The shell provides features like command execution, scripting capabilities, variable handling, and more.<br>
Different shells have different features and syntax. Common Unix-like shells include the original Bourne shell or sh; the C shell or csh; the Korn shell or ksh; the Z shell or zsh; as well as the bash shell (Bourne-Again SHell) which is our foucus here.. Windows systems use shells like Command Prompt and PowerShell.<br>
The shell's primary function is to interpret and execute the commands you enter.<br>

## Shell commands vs. Python functions
Both shell commands and Python functions are executed to perform specific actions or tasks, but they have distinct purposes, characteristics, and use cases. In Python, functions are for organizing the program, but Shell commands run programs. <br>
In other words, Shell commands are executed within the shell environment of the operating system. They interact directly with the system and perform tasks such as file manipulation, system configuration, and process management.
However, Python functions are part of a Python script or program. They execute within the Python interpreter and are used for defining reusable blocks of code that can perform specific tasks.

## Tips
`tab`: autocompletes names.<br>
`Ctrl + C`: sends an interrupt signal to the currently running process. This is often used to forcefully terminate a command that is taking too long or is stuck.<br>
`Ctrl + Z`: is used to suspend a currently running foreground process and return control to the shell. This is often used to temporarily pause a process.<br>
`Ctrl + D`: indicates an "end-of-file" (EOF) condition to the shell. It can be used to exit certain interactive commands, such as text editors like nano, or to signal the end of input for a command.<br>
Type `exit`: For some interactive programs, typing the word `exit` and pressing Enter will close the program and return you to the shell prompt. This works for commands like `python` (Python interpreter) and `irb` (Ruby interpreter).

## Popular commands
`ls`: displays the names of files and directories within the current working directory. `ls -a` prints out all files in the direcotry including hidden files (directories that have names starting with a dot `.`)<br>
`cat`: is used to concatenate and display the contents of files. Its primary function is to read one or more files and display their contents in the terminal. For example: `cat file1.txt file2.txt`<br>
`unzip`: allows you to decompress and restore the original files and directory structure that were compressed into the archive.<br>
`wc`: stands for "word count", but it provides more than just word counting. It is a simple yet versatile tool for basic text analysis including number of lines, words, and bytes.<br>
`diff`: is used to compare the content of two text files or directories and display the differences between them. It is commonly used to identify changes made to files, configurations, or code over time. The output of the diff command highlights the lines or sections that differ between the files being compared. For example `diff file1.txt file1_draft.txt`<br>
`man`: is used to display the manual pages (also known as "man pages") for other commands, programs, and system functions. Man pages provide detailed documentation and information about how to use various commands and utilities available in the operating system. For example: `man ls`<br>
`nano`: is a simple and user-friendly text editor that is commonly used in Unix and Unix-like operating systems, including Linux. It provides a command-line interface for editing text files directly from the terminal. `nano` is particularly popular among users who are new to the command line and want a straightforward and intuitive text editor. E.g., `nano file_name`

## Filesystem Tree
The filesystem tree, also known as the directory tree or directory structure, is a hierarchical organization of files and directories (folders) on a computer's storage system. It represents how files and directories are organized and stored within an operating system.

In a filesystem tree:

* **Root Directory:** At the top level is the root directory, often represented by a forward slash ("/") in Unix-like systems (Linux, macOS) or a drive letter (e.g., "C:") in Windows. The root directory contains all other directories and files.
* **Directories (Folders):** Directories, also known as folders, are containers that hold files and other directories. They can be nested within each other to create a hierarchical structure.
* **Files:** Files are individual units of data that contain content. They are organized within directories based on the needs and organization of the system and its users.
* **Path:** The path is a sequence of directory names separated by slashes ("/" in Unix-like systems) that specifies the location of a file or directory within the filesystem tree. An absolute path starts from the root directory, while a relative path starts from the current working directory.

`pwd`: stands for "print working directory". When you run the pwd command in a terminal or command prompt, it displays the current directory or the path of the directory you are currently located in. An example output is: `/users/Abed`<br>
`cd`: is used to **C**hange the current working **D**irectory in a Unix, Unix-like, or Windows command prompt environment. It allows you to navigate and switch between different directories within the file system. E.g., `cd Music`<br>
`cd ..`: is used to navigate to the parent directory (also known as the "parent folder" or "up one level") in a file system using a command-line interface. It is a common command used in terminal or command prompt environments to move from a current directory to the directory that contains it.<br>
`cd /`: changes the current working directory to the root directory of the file system.<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

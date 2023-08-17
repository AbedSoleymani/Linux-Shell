# Linux-Shell

## Distribution families
In the Linux ecosystem, distributions are often grouped into families based on their common origins, design philosophies, and package management systems. Here are the Red Hat family, SUSE, and Debian families explained:

1. **Red Hat Family:**
The Red Hat family includes Linux distributions that are based on the work of Red Hat Inc. These distributions typically use the Red Hat Package Manager (RPM) for package management. Red Hat Enterprise Linux (RHEL) is the flagship distribution in this family, known for its stability and focus on enterprise use. CentOS, a free and open-source version of RHEL, was also part of this family until its shift to CentOS Stream. Other notable members of the Red Hat family include Fedora (a community-driven distribution sponsored by Red Hat) and CentOS Stream (a rolling-release version aligned with RHEL development).
2. **SUSE Family:**
The SUSE family encompasses distributions developed by SUSE, a prominent Linux vendor. SUSE distributions are known for their flexibility and are widely used in enterprise environments. SUSE Linux Enterprise Server (SLES) is a key member of this family, offering robust features for businesses. openSUSE, a community-driven distribution, is also part of the SUSE family and is available in both Leap (stable) and Tumbleweed (rolling-release) versions.
3. **Debian Family:**
The Debian family includes distributions that are derived from Debian, an influential and widely respected community-driven distribution. Debian is known for its commitment to free software and its strong package management system (APT). Ubuntu, one of the most popular Linux distributions, is based on Debian and is designed for usability and ease of use. Many other distributions, such as Linux Mint and MX Linux, are also based on Debian.

Each family has its own characteristics, strengths, and focus areas, catering to a diverse range of users and use cases within the Linux ecosystem.

## Linux Terminologies
1. **Kernel:**
The kernel is the core component of the Linux operating system. It acts as a bridge between hardware and software, managing system resources, handling hardware communication, and providing essential services to other software components. It enables processes to run, manages memory, controls input/output operations, and maintains security.
2. **Distribution (Distro):**
A Linux distribution is a complete operating system that includes the Linux kernel along with a collection of software packages, libraries, utilities, and tools. Different distributions offer various configurations, package managers, and user interfaces, catering to specific use cases and user preferences.
3. **Boot Loader:**
The boot loader is a program that manages the boot process of the operating system. It resides in the computer's master boot record (MBR) and is responsible for loading the operating system kernel into memory from storage. Popular Linux boot loaders include GRUB (GRand Unified Bootloader) and LILO (Linux Loader).
4. **Service:**
In the context of Linux, a service refers to a background process or program that performs specific tasks, such as networking, file sharing, or system management. Services can be started, stopped, and managed to ensure the proper functioning of the system. Example: httpd, nfsd, ntpd, ftpd and named.
5. **Filesystem:**
The filesystem is a method used to organize and store files on a storage device, such as a hard drive or SSD. It determines how files are named, organized, accessed, and stored on the storage medium. Common Linux filesystems include ext4, XFS, and Btrfs.
6. **Window System:**
The window system is a software component that manages graphical user interfaces (GUIs) by providing a framework for creating, displaying, and interacting with windows, icons, menus, and other graphical elements on the screen. X Window System (X11) and its modern successor Wayland are popular window systems used in Linux.
7. **Desktop Environment:**
A desktop environment is a complete graphical interface that provides a user-friendly environment for interacting with the computer. It includes a window manager, panel, file manager, and various applications. Examples of Linux desktop environments include GNOME, KDE Plasma, and XFCE.
8. **Command Line:**
The command line, also known as the terminal or shell, is a text-based interface for interacting with the Linux operating system using commands. Users can type commands to perform tasks, manage files, install software, configure settings, and perform various system operations.

## Terminal
A **terminal**, also known as a **command-line interface (CLI)**, **shell**, or **console**, is a text-based interface used to interact with a computer's operating system and execute commands. It provides a way to communicate with the computer using text commands rather than a graphical user interface (GUI).

In a terminal, you can enter commands and receive text-based responses from the computer. This allows you to perform various tasks, such as navigating the file system, running programs, managing files and directories, configuring system settings, and more. Terminals are commonly used in programming, system administration, and various technical tasks.

Although GUI interfaces are quite easy to use, they are not as flexible as the command line. Imagine copying a thousand files with a GUI. It would take a few clicks to select the files, some scrolling and some to and fro between the source and target directories. Doing the same thing from command line involves a fair bit of typing. So the command line approach may not seem a clear winner. Now consider renaming files in bulk or separating them based on their timestamps. It is tough to perform tasks like these from the GUI because GUIs are not programmable. With the command line you can combine multiple commands to, for example, find the timestamp, and copy the files based on the timestamps.

A good command line interface, like the Linux shell allows you to write scripts to automate tasks like these. In fact, the Linux shell comes with a long list of commands that can be composed to automate any task imaginable. This ability to build larger programs from smaller ones is what gives the command line its power and flexibility.

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
`tab`: autocompletes names.<br><br>
`Ctrl + C`: sends an interrupt signal to the currently running process. This is often used to forcefully terminate a command that is taking too long or is stuck.<br><br>
`Ctrl + Z`: is used to suspend a currently running foreground process and return control to the shell. This is often used to temporarily pause a process.<br><br>
`Ctrl + D`: indicates an "end-of-file" (EOF) condition to the shell. It can be used to exit certain interactive commands, such as text editors like nano, or to signal the end of input for a command.<br><br>
Type `exit`: For some interactive programs, typing the word `exit` and pressing Enter will close the program and return you to the shell prompt. This works for commands like `python` (Python interpreter) and `irb` (Ruby interpreter).

## Popular commands
`ls`: displays the names of files and directories within the current working directory. `ls -a` prints out all files in the direcotry including hidden files (directories that have names starting with a dot `.`)<br><br>
`cat`: is used to concatenate and display the contents of files. Its primary function is to read one or more files and display their contents in the terminal. For example: `cat file1.txt file2.txt`<br>
`head -n 20 file.txt` will display the first 20 lines of the file `file.txt`<br>
`tail` command displays the last few lines of a text file. By default, it shows the last 10 lines, but you can specify a different number of lines using the `-n` option. Additionally, you can use the `-f` option to continuously monitor a file and display new lines as they are added (useful for log files: `tail -f logfile.log`).<br>
`less`: Both `cat` and `less` are commands used in Unix-like operating systems to view the contents of text files in the terminal. However, they have different functionalities and use cases. `less` is a more advanced command that allows you to view and navigate through the contents of a file in a pager-like manner. It is particularly useful for viewing large files. `less` displays the content of the file one screen at a time, allowing you to scroll up and down, search, and navigate within the file. Example: `less large_file.txt`
It provides various keyboard shortcuts for navigation and interaction, such as arrow keys, page up, page down, searching, and quitting.<br><br>
`unzip`: allows you to decompress and restore the original files and directory structure that were compressed into the archive.<br><br>
`wc`: stands for "word count", but it provides more than just word counting. It is a simple yet versatile tool for basic text analysis including number of lines, words, and bytes.<br><br>
`grep`: is used to search for specified patterns or text strings within files or the output of other commands. It stands for "Global Regular Expression Print," and it is commonly used for text processing and pattern matching. Example: `grep "error" log.txt`<br><br>
`diff`: is used to compare the content of two text files or directories and display the differences between them. It is commonly used to identify changes made to files, configurations, or code over time. The output of the diff command highlights the lines or sections that differ between the files being compared. For example `diff file1.txt file1_draft.txt`<br><br>
`man`: is used to display the manual pages (also known as "man pages") for other commands, programs, and system functions. Man pages provide detailed documentation and information about how to use various commands and utilities available in the operating system. For example: `man ls`<br><br>
`nano`: is a simple and user-friendly text editor that is commonly used in Unix and Unix-like operating systems, including Linux. It provides a command-line interface for editing text files directly from the terminal. `nano` is particularly popular among users who are new to the command line and want a straightforward and intuitive text editor. E.g., `nano file_name`<br><br>
`echo`: is used to display text or output to the terminal or command-line interface. When you use the echo command, the specified text or variables are printed to the screen. It is often used for displaying messages, variable values, or generating simple output. E.g., `echo "Hello, world!"` or:<br>
`name="John"`<br>
`echo "My name is $name."`<br><br>
`curl`: allows you to transfer data to or from a network server using various protocols. It stands for "**Client URL**" and is used primarily to perform HTTP requests, although it supports several other network protocols as well. For instance<br><br>
`curl -O https://example.com/file.zip`<br>
downloads the file `file.zip` from `https://example.com` and saves it in the current directory.

## Filesystem Tree
The filesystem tree, also known as the directory tree or directory structure, is a hierarchical organization of files and directories (folders) on a computer's storage system. It represents how files and directories are organized and stored within an operating system.

In a filesystem tree:

* **Root Directory:** At the top level is the root directory, often represented by a forward slash ("/") in Unix-like systems (Linux, macOS) or a drive letter (e.g., "C:") in Windows. The root directory contains all other directories and files.
* **Directories (Folders):** Directories, also known as folders, are containers that hold files and other directories. They can be nested within each other to create a hierarchical structure.
* **Files:** Files are individual units of data that contain content. They are organized within directories based on the needs and organization of the system and its users.
* **Path:** The path is a sequence of directory names separated by slashes ("/" in Unix-like systems) that specifies the location of a file or directory within the filesystem tree. An absolute path starts from the root directory, while a relative path starts from the current working directory.

`pwd`: stands for "print working directory". When you run the pwd command in a terminal or command prompt, it displays the current directory or the path of the directory you are currently located in. An example output is: `/users/Abed`<br><br>
`cd`: is used to **C**hange the current working **D**irectory in a Unix, Unix-like, or Windows command prompt environment. It allows you to navigate and switch between different directories within the file system. E.g., `cd Music`<br><br>
`cd ..`: is used to navigate to the parent directory (also known as the "parent folder" or "up one level") in a file system using a command-line interface. It is a common command used in terminal or command prompt environments to move from a current directory to the directory that contains it.<br><br>
`cd /`: changes the current working directory to the root directory of the file system.<br><br>
`cd+Enter`: Typing `cd` followed by the `Enter` key alone without specifying a directory or path is a way to quickly return to your home directory in which you started your terminal.<br><br>
`cd .`: is used to change the current directory to the current directory itself. In other words, it doesn't actually change the directory; it remains in the same directory.<br><br>
`mv`: move! After using `mv`, the original file or directory is no longer present at the source location.
*  It is used to move files or directories from one location to another, essentially changing their location in the file system: `mv file.txt /path/to/new/location/`
* t can also be used to rename files or directories by specifying a new name during the move: `mv oldname.txt newname.txt`

`cp`: copy! Unlike `mv`, the original file or directory remains intact at the source location.
* It is used to copy files or directories from one location to another, creating a duplicate of the original file or directory at the destination: `cp file.txt /path/to/destination/`
* It can be used to copy a single file, multiple files, or entire directories: `cp -r source/* destination/` in which `-r` means recursively copy (or move) directories and their contents.

`mkdir`: is used to create new directories (also known as folders) within the file system. E.g., `mkdir directory_name`. Please note that this directory used relative path. We can use absolute path as well: `mkdir /users/Abed/new_direcotry`<br><br>
`rmdir`: is used to remove (delete) **_empty_** directories from the file system. It stands for "remove directory." Unlike the `rm` command, which is used to remove files and directories, `rmdir` is specifically designed to remove only directories that are empty. E.g., `rmdir empty_direcotry`. To remove a directory and all of its contents, we can use `rm -r directory_name`
## Globbing
is a feature of Unix and Unix-like shells that allows you to use special characters called wildcards to match and manipulate filenames and paths. These wildcards enable you to perform various operations on files and directories that match a specified pattern. For instance:
* `ls *html` returns: `app.html` and `index.html`
* `ls app*` returns: `app.html`, `app.css`, `app.js`
* `ls *s` returns: `app.css` and `app.js`
* `ls *pp*` returns: `app.html`, `app.css`, `app.js`
* `ls app.{html,css}` returns: `app.html`, `app.css`
* `ls bea?.png` returns `bean.png` and `bear.png`
* `ls *.{jpg,JPG}`

# Linux Navigation Basics: Basic Commands

Linux Navigation Basics is about using simple commands to move around and manage files on your computer. 
For example, cd lets you go into different folders, ls shows you what files and folders are inside, and pwd tells you where you are currently. These commands help you easily find and organize your files.

# pwd (Print Working Directory)
Shows the full path of your current directory.
```bash
pwd
Output: /home/username/Desktop
```
# ls (List)
Lists files and subdirectories in the current directory.
+ `ls -l` : Detailed list including Permissions, Owner, Size, Modification Time.
+ `ls -a` : Include hidden files (starting with `.`).
+ `ls -lh`: Detailed list including Permissions, Owner, Size, Modification Time but contain human-readable file sizes (e.g., 4K, 2M).
+ `ls -t` : Sort by modification time (newest first).
+ `ls -r` : Recursively list subdirectories.

# cd (Change Directory)
Move between directories.
+ `cd` or `cd ~`    : Go to your home directory.
+ `cd ..`           : Switch to previous directory.
+ `cd /path`        : Absolute path because it starts from root `/` directory (e.g., cd /etc).
+ `cd relative/path`: Relative to current directory (e.g., cd Documents/Projects).

# Key Shortcuts
+ `~` : Your home directory.
+ `.` : Current directory
+ `..`: Parent directory.

# Tips
+ **Tab Completion**: Type part of a directory name and press Tab to auto-complete.
+ **Wildcards**: Use `*` to match patterns (e.g., ls *.txt lists all text files).
+ **Case Sensitivity**: Linux paths are case-sensitive (`Documents` ≠ `documents`).

In this brief introduction, we will discuss and explore these basic commands and how they aid us in navigation around the Linux environment.

Learn more from the following resources:
+ [@article@ Linux Navigation Basics](https://labex.io/tutorials/linux-file-and-directory-operations-17997)

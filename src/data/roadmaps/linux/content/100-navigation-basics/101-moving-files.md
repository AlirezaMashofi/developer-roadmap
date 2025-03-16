# Move/Rename Files/Directories

In Linux, moving files is an essential task that you will need to perform quite frequently. The `mv` command, short for move, is used to move files and directories from one location to another. The `mv` command can also be used for renaming files in Linux.

# Syntax
```bash
mv [options] <source> <destination>
```
+ `source`     : Denotes the file or directory that you want to move.
+ `destination`: Denotes the location where you want to move your source file or directory.
+ `options`    : Key options are as follows 

| Option | Purpose |
| :---   | :---    |
| `-i`   | **Interactive**: Prompt before overwriting existing files.            |
| `-v`   | **Verbose:** Show details of the operation.                           |
| `-n`   | **No Overwrite**: Skip moving if the destination file already exists. |
| `-u`   | **Update**: Move only if the source is newer than the destination.    |

# Use Cases
**1. Rename a File**
```bash
mv old_name.txt new_name.txt           # Rename "old_name.txt" to "new_name.txt"
```
**2. Move a File to Another Directory**
```bash
mv file.txt /path/destination/         # Move "file.txt" to the destination folder
```
**3. Move Multiple Files to a Directory**
```bash
mv file_1.txt file_2.jpg ~/Documents/  # Move both files to "Documents"
```
**4. Move All Files in a Directory**
```bash
mv *.png ~/Pictures/                   # Move all PNG files to "Pictures"
mv ../Downloads/*.mp3 .                # Move MP3s from Downloads to the current directory
```
**5. Move and Rename in One Step**
```bash
mv report.txt /backup/report_2024.txt  # Move and rename simultaneously
```
**6. Move Hidden Files**
mv .hidden_file ~/.config/             # Move hidden files/directories
**7. Move or Rename Directories**
```bash
mv old_dir/ new_dir/                   # Rename or Move a directory
```
# Safet Tips
+ **Avoid Overwrites**: Use `-i` to confirm before replacing files.
```bash
mv -i important.txt ~/Documents/       # Confirm if "important.txt" exists there
```
Without `-i`, `mv` silently overwrites existing files.
+ **Backup First**: Use `--backup` to create backups of overwritten files.
```bash
mv --backup=numbered file.txt ~/       # Creates `file.txt.~1~`, etc.
```
+ **Trailing Slashes**: `mv dir1/ dir2/` vs. `mv dir1 dir2` (slashes matter if dir2 exists).
+ **Wildcards in Wrong Directories**: Ensure you’re in the correct folder before running `mv *.txt`.
+ **Check Permissions**: Ensure you have write access to both the source and destination.

Use `mv` for simple moves/renames and combine it with wildcards or scripts for efficiency

Learn more from the following resources:

- [@article@Linux mv Command: File Moving and Renaming](https://labex.io/tutorials/linux-linux-mv-command-file-moving-and-renaming-209743)

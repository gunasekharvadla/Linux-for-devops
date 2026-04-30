📂 File & Directory Management in Linux
===================================================
📁 Basic File and Directory Operations

| Command                  | Description                                         |
| ------------------------ | --------------------------------------------------- |
| `ls`                     | Lists files and directories in the current location |
| `cd /path/to/directory`  | Changes the working directory                       |
| `pwd`                    | Displays the current working directory              |
| `mkdir new_folder`       | Creates a new directory                             |
| `rmdir empty_folder`     | Removes an empty directory                          |
| `rm file.txt`            | Deletes a file                                      |
| `rm -r folder`           | Deletes a folder and its contents recursively       |
| `cp file1.txt file2.txt` | Copies a file                                       |
| `cp -r dir1 dir2`        | Copies a directory recursively                      |
| `mv old_name new_name`   | Moves or renames a file/directory                   |


=================================================================

📄 File Viewing and Editing

| Command                    | Description                                                  |
| -------------------------- | ------------------------------------------------------------ |
| `cat file.txt`             | Displays file content                                        |
| `tac file.txt`             | Displays file content in reverse order                       |
| `less file.txt`            | Opens file with scroll support (recommended for large files) |
| `more file.txt`            | Opens file (forward navigation only)                         |
| `head -n 10 file.txt`      | Shows first 10 lines                                         |
| `tail -n 10 file.txt`      | Shows last 10 lines                                          |
| `nano file.txt`            | Opens file in simple text editor                             |
| `vi file.txt`              | Opens file in advanced text editor                           |
| `echo 'Hello' > file.txt`  | Writes text (overwrites file)                                |
| `echo 'Hello' >> file.txt` | Appends text to file                                         |


==========================================================================


📌 Example Workflow

mkdir project

cd project

echo "Hello Linux" > file.txt

cat file.txt

cp file.txt backup.txt

ls

rm backup.txt











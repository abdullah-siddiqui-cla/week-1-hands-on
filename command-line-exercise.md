# Command Line Exercise

This exercise will help you practice basic command-line operations. Follow the instructions step by step.

**Note:** Instructions are provided for both **Mac/Linux** and **Windows Command Prompt**. Use the commands that match your operating system.

## Prerequisites
- Open your terminal/command prompt
- Navigate to a practice directory (you can create one with `mkdir practice` and then `cd practice`)

---

## Exercise 1: `pwd` - Print Working Directory

**Task:** Find out where you are in the file system.

**Mac/Linux:**
1. Type `pwd` and press Enter
2. Note the current directory path

**Windows:**
1. Type `cd` (with no arguments) and press Enter
2. Note the current directory path

**Expected Output:** A path showing your current location (e.g., `/Users/yourname/practice` on Mac/Linux, or `C:\Users\yourname\practice` on Windows)

---

## Exercise 2: `cd` - Change Directory

**Task:** Navigate through directories.

**Mac/Linux:**
1. Go to your home directory: `cd ~` or `cd`
2. Check your location: `pwd`
3. Go back to the practice directory: `cd practice` (or `cd /path/to/practice`)
4. Try going up one directory: `cd ..`
5. Check your location again: `pwd`
6. Return to the practice directory: `cd practice`

**Windows:**
1. Go to your home directory: `cd %USERPROFILE%` or `cd`
2. Check your location: `cd`
3. Go back to the practice directory: `cd practice` (or `cd C:\path\to\practice`)
4. Try going up one directory: `cd ..`
5. Check your location again: `cd`
6. Return to the practice directory: `cd practice`

---

## Exercise 3: `ls` / `dir` - List Directory Contents

**Task:** View files and directories.

**Mac/Linux:**
1. List all files and directories: `ls`
2. List with details (long format): `ls -l`
3. List all files including hidden ones: `ls -a`
4. List with human-readable sizes: `ls -lh`
5. List in reverse order: `ls -r`

**Windows:**
1. List all files and directories: `dir`
2. List with details (long format): `dir`
3. List all files including hidden ones: `dir /a`
4. List with human-readable sizes: `dir`
5. List in reverse order: `dir /o-n`

---

## Exercise 4: `touch` - Create Empty Files

**Task:** Create new empty files.

**Mac/Linux:**
1. Create a file named `file1.txt`: `touch file1.txt`
2. Create multiple files at once: `touch file2.txt file3.txt file4.txt`
3. Verify the files were created: `ls`

**Windows:**
1. Create a file named `file1.txt`: `type nul > file1.txt`
2. Create multiple files at once: `type nul > file2.txt` then `type nul > file3.txt` then `type nul > file4.txt`
   - Or use: `echo. > file2.txt` and `echo. > file3.txt` and `echo. > file4.txt`
3. Verify the files were created: `dir`

---

## Exercise 5: `echo` - Display Text

**Task:** Use echo to display and write text.

**Mac/Linux:**
1. Display text to the terminal: `echo "Hello, World!"`
2. Write text to a file: `echo "This is my first file" > file1.txt`
3. Append text to a file: `echo "This is a second line" >> file1.txt`
4. Display the contents: `cat file1.txt`

**Windows:**
1. Display text to the terminal: `echo Hello, World!`
2. Write text to a file: `echo This is my first file > file1.txt`
3. Append text to a file: `echo This is a second line >> file1.txt`
4. Display the contents: `type file1.txt`

---

## Exercise 6: `cat` / `type` - Display File Contents

**Task:** View file contents.

**Mac/Linux:**
1. Display the contents of `file1.txt`: `cat file1.txt`
2. Display multiple files: `cat file1.txt file2.txt`
3. Create content in `file2.txt`: `echo "Content for file 2" > file2.txt`
4. Display both files: `cat file1.txt file2.txt`
5. Display with line numbers: `cat -n file1.txt`

**Windows:**
1. Display the contents of `file1.txt`: `type file1.txt`
2. Display multiple files: `type file1.txt file2.txt`
3. Create content in `file2.txt`: `echo Content for file 2 > file2.txt`
4. Display both files: `type file1.txt file2.txt`
5. Display with line numbers: `find /n /v "" file1.txt`

---

## Exercise 7: `mkdir` - Create Directories

**Task:** Create new directories.

**Mac/Linux:**
1. Create a directory named `test`: `mkdir test`
2. Create multiple directories: `mkdir dir1 dir2 dir3`
3. Create nested directories: `mkdir -p test/subdir1/subdir2`
4. List directories: `ls -l`

**Windows:**
1. Create a directory named `test`: `mkdir test`
2. Create multiple directories: `mkdir dir1 dir2 dir3`
3. Create nested directories: `mkdir test\subdir1\subdir2`
4. List directories: `dir`

---

## Exercise 8: `cp` / `copy` - Copy Files and Directories

**Task:** Copy files and directories.

**Mac/Linux:**
1. Copy `file1.txt` to `file1_copy.txt`: `cp file1.txt file1_copy.txt`
2. Verify the copy: `ls` and `cat file1_copy.txt`
3. Copy a file to a directory: `cp file2.txt test/`
4. Copy a directory recursively: `cp -r dir1 test/`
5. Verify: `ls test/`

**Windows:**
1. Copy `file1.txt` to `file1_copy.txt`: `copy file1.txt file1_copy.txt`
2. Verify the copy: `dir` and `type file1_copy.txt`
3. Copy a file to a directory: `copy file2.txt test\`
4. Copy a directory recursively: `xcopy dir1 test\dir1 /e /i`
5. Verify: `dir test`

---

## Exercise 9: `mv` / `move` / `ren` - Move/Rename Files and Directories

**Task:** Move and rename files.

**Mac/Linux:**
1. Rename `file3.txt` to `renamed_file.txt`: `mv file3.txt renamed_file.txt`
2. Verify: `ls`
3. Move `file4.txt` into the `test` directory: `mv file4.txt test/`
4. Verify: `ls` and `ls test/`
5. Move a directory: `mv dir2 test/`
6. Verify: `ls test/`

**Windows:**
1. Rename `file3.txt` to `renamed_file.txt`: `ren file3.txt renamed_file.txt`
2. Verify: `dir`
3. Move `file4.txt` into the `test` directory: `move file4.txt test\`
4. Verify: `dir` and `dir test`
5. Move a directory: `move dir2 test\`
6. Verify: `dir test`

---

## Exercise 10: `rmdir` - Remove Empty Directories

**Task:** Remove empty directories.

**Mac/Linux:**
1. Try to remove an empty directory: `rmdir dir3`
2. Verify it's gone: `ls`
3. Try to remove a non-empty directory (this will fail): `rmdir test`
4. Note: You'll need to use `rm -r` for non-empty directories

**Windows:**
1. Try to remove an empty directory: `rmdir dir3`
2. Verify it's gone: `dir`
3. Try to remove a non-empty directory (this will fail): `rmdir test`
4. Note: You'll need to use `rmdir /s` or `rd /s` for non-empty directories

---

## Exercise 11: `rm` / `del` - Remove Files and Directories

**Task:** Delete files and directories.

**Mac/Linux:**
1. Remove a file: `rm file1_copy.txt`
2. Verify: `ls`
3. Remove multiple files: `rm file2.txt renamed_file.txt`
4. Remove a directory and its contents: `rm -r dir1`
5. Remove a directory forcefully: `rm -rf test/subdir1` (be careful with this!)
6. Verify: `ls -R test/`

**Windows:**
1. Remove a file: `del file1_copy.txt`
2. Verify: `dir`
3. Remove multiple files: `del file2.txt renamed_file.txt`
4. Remove a directory and its contents: `rmdir /s dir1`
5. Remove a directory forcefully: `rmdir /s /q test\subdir1` (be careful with this!)
6. Verify: `dir /s test`

---

## Challenge Exercise: Putting It All Together

**Task:** Complete this sequence of commands:

**Mac/Linux:**
1. Create a directory called `project`
2. Navigate into it: `cd project`
3. Create three files: `touch readme.txt notes.txt todo.txt`
4. Add content to `readme.txt`: `echo "Project Readme" > readme.txt`
5. Add content to `notes.txt`: `echo "My notes" > notes.txt`
6. Create a subdirectory: `mkdir docs`
7. Copy `readme.txt` to the `docs` directory: `cp readme.txt docs/`
8. Rename `notes.txt` to `notes_backup.txt`: `mv notes.txt notes_backup.txt`
9. List all files with details: `ls -lh`
10. Display the contents of `readme.txt` using `cat`: `cat readme.txt`
11. Go back to the parent directory: `cd ..`
12. Remove the entire `project` directory: `rm -r project`

**Windows:**
1. Create a directory called `project`
2. Navigate into it: `cd project`
3. Create three files: `type nul > readme.txt` then `type nul > notes.txt` then `type nul > todo.txt`
4. Add content to `readme.txt`: `echo Project Readme > readme.txt`
5. Add content to `notes.txt`: `echo My notes > notes.txt`
6. Create a subdirectory: `mkdir docs`
7. Copy `readme.txt` to the `docs` directory: `copy readme.txt docs\`
8. Rename `notes.txt` to `notes_backup.txt`: `ren notes.txt notes_backup.txt`
9. List all files with details: `dir`
10. Display the contents of `readme.txt` using `type`: `type readme.txt`
11. Go back to the parent directory: `cd ..`
12. Remove the entire `project` directory: `rmdir /s project`

---

## Tips

**Mac/Linux:**
- Use `man <command>` to see the manual page for any command (e.g., `man ls`)
- Use `Tab` key for auto-completion
- Use `Ctrl+C` to cancel a running command
- Use `history` to see your previous commands
- Use `clear` to clear the terminal screen

**Windows:**
- Use `help <command>` or `<command> /?` to see help (e.g., `help dir` or `dir /?`)
- Use `Tab` key for auto-completion
- Use `Ctrl+C` to cancel a running command
- Use `doskey /history` to see your previous commands
- Use `cls` to clear the terminal screen

---

## Review Questions

1. What's the difference between `cp` and `mv`?
2. When would you use `rmdir` vs `rm -r`?
3. What does `>>` do differently than `>` with the `echo` command?
4. How do you create a directory structure like `a/b/c` in one command?
5. What's the difference between `cd ~` and `cd ..`?

---

Good luck with your practice! 🚀


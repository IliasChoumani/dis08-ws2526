# 🐧 Linux Journey – The Shell
## Quiz Answers (Lessons 1–19)
**Course:** DIS08 – Datenmodellierung Lab 03
**Student:** Ilias Choumani
**Date:** November 2025  

---

### 1. What is the exact output to the display when you type `echo Hello World`?
**Answer:**  
```
Hello World
```

**Example:**
```bash
echo Hello World
# Output: Hello World
```

---

### 2. Which command is used to find the directory you are currently in?
**Answer:**  
```
pwd
```

**Explanation:**  
The command `pwd` (print working directory) displays the full path of your current directory.

**Example:**
```bash
pwd
# Output: /home/ilias
```

---

### 3. If you are in `/home/pete/Pictures` and want to navigate to the parent directory (`/home/pete`), what is the full command you should use?
**Answer:**  
```
cd ..
```

**Explanation:**  
Two dots (`..`) represent the parent directory in Linux.

**Example:**
```bash
cd /home/pete/Pictures
cd ..
# Now in: /home/pete
```

---

### 4. What command would you use to see hidden files?
**Answer:**  
```
ls -a
```

**Explanation:**  
Hidden files begin with a dot (`.`). The `-a` flag lists **all** files, including hidden ones.

**Example:**
```bash
ls -a
# Output: .bashrc  .hiddenfile  Documents  Pictures
```

---

### 5. How do you create a file called `myfile`?
**Answer:**  
```
touch myfile
```

**Explanation:**  
The `touch` command creates an empty file or updates an existing file’s timestamp.

**Example:**
```bash
touch myfile
ls
# Output: myfile
```

---


### 6. What command can you use to find the file type of a file?
**Answer:**  
```
file
```

**Explanation:**  
The `file` command determines the type of a given file based on its content.

**Example:**
```bash
file myfile
# Output: myfile: ASCII text
```

---

### 7. What command is used to display the contents of a file on the command line?
**Answer:**  
```
cat
```

**Explanation:**  
The `cat` command (short for *concatenate*) is used to display the contents of one or more files directly in the terminal.

**Example:**
```bash
cat myfile
# Output: Hello World
```

---

### 8. How do you quit out of the `less` command?
**Answer:**  
```
q
```

**Explanation:**  
While using `less`, press the **q** key to quit and return to the command prompt.

**Example:**
```bash
less myfile
# (viewing file)
# Press 'q' to quit
```

---

### 9. What is the command to clear the terminal?
**Answer:**  
```
clear
```

**Explanation:**  
The `clear` command removes all previous text from the terminal display.

**Example:**
```bash
clear
# Screen cleared
```

---

### 10. What flag do you need to specify to copy over a directory?
**Answer:**  
```
-r
```

**Explanation:**  
The `-r` (recursive) flag is required with the `cp` command to copy directories and their contents.

**Example:**
```bash
cp -r mydir backup/
# Copies 'mydir' and all its files into 'backup/'
```

---


### 11. Using the `mv` command, how would you rename a file named `cat` to `dog`?
**Answer:**  
```
mv cat dog
```

**Explanation:**  
The `mv` command moves or renames files. Here, it renames the file `cat` to `dog`.

**Example:**
```bash
mv cat dog
ls
# Output: dog
```

---

### 12. What command is used to make a directory?
**Answer:**  
```
mkdir
```

**Explanation:**  
The `mkdir` command creates a new directory (folder).

**Example:**
```bash
mkdir new_folder
ls
# Output: new_folder
```

---

### 13. How do you remove a file named `myfile`?
**Answer:**  
```
rm myfile
```

**Explanation:**  
The `rm` (remove) command deletes files from the filesystem.

**Example:**
```bash
rm myfile
ls
# Output: (file no longer listed)
```

---

### 14. What option should you specify for the `find` command to search by name?
**Answer:**  
```
-name
```

**Explanation:**  
The `-name` option allows you to search for files matching a specific name pattern.

**Example:**
```bash
find . -name "example.txt"
# Output: ./Documents/example.txt
```

---

### 15. How do you get quick command-line help for built-in Bash commands?
**Answer:**  
```
help
```

**Explanation:**  
The `help` command displays quick usage information for Bash built-in commands.

**Example:**
```bash
help cd
# Output: cd: cd [-L|[-P [-e]] [-@]] [dir]
#       Change the shell working directory.
```

---


### 16. How do you see the manual for a command?
**Answer:**  
```
man
```

**Explanation:**  
The `man` command opens the manual page for another command, showing its description, syntax, and options.

**Example:**
```bash
man ls
# Output: Displays the manual for the 'ls' command
```

---

### 17. What command can you use to see a small description of a command?
**Answer:**  
```
whatis
```

**Explanation:**  
The `whatis` command gives a brief, one-line summary of what a command does.

**Example:**
```bash
whatis pwd
# Output: pwd (1) - print name of current/working directory
```

---

### 18. What command is used to create an alias?
**Answer:**  
```
alias
```

**Explanation:**  
The `alias` command lets you define shortcuts for other commands.

**Example:**
```bash
alias ll='ls -la'
ll
# Output: Lists all files including hidden ones in long format
```

---

### 19. What is the most common command to exit from the Linux shell?
**Answer:**  
```
exit
```

**Explanation:**  
The `exit` command ends the current shell session and closes the terminal window.

**Example:**
```bash
exit
# Terminal session closed
```

---

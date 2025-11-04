# 🐧 Linux Journey – The Shell
## Quiz Answers (Lessons 1–5)
**Course:** DIS08 – Datenmodellierung (Bonusaufgabe)  
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
# Output: /home/liam
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

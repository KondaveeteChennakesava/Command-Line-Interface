# 🐧 Linux Command Quick Revision Notes

## 📁 Directory Management

| **Command**      | **Description**                        |
|------------------|----------------------------------------|
| `mkdir <name>`   | Create a new directory                 |
| `cd <name>`      | Navigate into the specified directory  |
| `cd ..`          | Navigate back to the parent directory  |
| `rm -R <name>`   | Recursively delete a directory         |
| `mv <old> <new>` | Rename or move a directory             |

---

## 📄 File Operations

| **Command**            | **Description**                          |
|------------------------|------------------------------------------|
| `touch <file>`         | Create a new file                        |
| `nano <file>`          | Open a file in `nano` editor             |
| `cat <file>`           | Display the contents of a file           |
| `mv <file> <dir>/`     | Move a file to a directory               |

---

## 🔍 Find and Delete Logs

| **Command**                                  | **Description**                                           |
|---------------------------------------------|-----------------------------------------------------------|
| `find . -name "*.log" -type f`              | List all `.log` files in current directory and subdirs    |
| `find . -name "*.log" -type f -delete`      | Delete all `.log` files from current directory recursively|

---

## 🔐 Permissions

| **Command**                            | **Description**                                    |
|----------------------------------------|----------------------------------------------------|
| `chmod 755 <file>`                     | Set file permissions to `rwxr-xr-x`                |
| `chmod -R 755 <directory>`             | Recursively set permissions for a directory        |

---

## ⚙️ System Information & Utilities

| **Command**         | **Description**                             |
|---------------------|---------------------------------------------|
| `ps -A` or `ps -e`  | Show all running processes                  |
| `firefox &`         | Launch Firefox in the background            |
| `whoami`            | Display current logged-in username          |
| `groups`            | Show groups the user belongs to             |
| `uname -m`          | Show machine hardware name (architecture)   |

---

## 📘 Download and Explore Book

| **Command**                                          | **Description**                                                   |
|------------------------------------------------------|-------------------------------------------------------------------|
| `curl -O https://www.gutenberg.org/cache/epub/223/pg223.txt` | Download the book                                                 |
| `head -n 3 pg223.txt`                                | Print the first 3 lines of the book                               |
| `tail -n 10 pg223.txt`                               | Print the last 10 lines of the book                               |
| `grep -o -i 'Harry' pg223.txt \| wc -l`              | Count occurrences of "Harry"                                      |
| `grep -o -i 'Ron' pg223.txt \| wc -l`                | Count occurrences of "Ron"                                        |
| `grep -o -i 'Hermione' pg223.txt \| wc -l`           | Count occurrences of "Hermione"                                   |
| `grep -o -i 'Dumbledore' pg223.txt \| wc -l`         | Count occurrences of "Dumbledore"                                 |
| `sed -n '100,200p' pg223.txt`                        | Print lines 100 through 200 in the book                           |
| `tr ' ' '\n' < pg223.txt \| tr -d '[:punct:]' \| tr 'A-Z' 'a-z' \| sort \| uniq \| wc -l` | Count unique words in the book  |

---

## 🧠 Processes and Ports

| **Command**                                      | **Description**                                                   |
|--------------------------------------------------|-------------------------------------------------------------------|
| `ps aux \| grep firefox`                         | List browser's process IDs and parent process IDs                 |
| `pkill firefox`                                  | Stop Firefox browser from command line                            |
| `ps -eo pid,ppid,%cpu,cmd --sort=-%cpu \| head -n 4` | List top 3 processes by CPU usage                              |
| `ps -eo pid,ppid,%mem,cmd --sort=-%mem \| head -n 4` | List top 3 processes by memory usage                           |

---

## 🌐 Python Server and Network

| **Command**                      | **Description**                                           |
|----------------------------------|-----------------------------------------------------------|
| `python3 -m http.server 8000`    | Start a Python HTTP server on port 8000                  |
| `lsof -i :8000`                  | Find PID of process on port 8000                         |
| `kill <PID>`                     | Stop Python HTTP server                                  |
| `python3 -m http.server 90`      | Start a Python HTTP server on port 90                    |
| `netstat -tuln`                  | Display all active connections and TCP/UDP ports         |
| `sudo lsof -i :5432`             | Find PID of process listening on port 5432               |

---

## 📦 Managing Software (Debian-based with apt)

| **Command**                           | **Description**                     |
|----------------------------------------|-------------------------------------|
| `sudo apt update`                      | Update package list                 |
| `sudo apt install htop vim nginx -y`  | Install htop, vim, and nginx        |
| `sudo apt remove nginx -y`            | Uninstall nginx                     |

---

## 🔍 Miscellaneous

| **Command**               | **Description**                            |
|---------------------------|--------------------------------------------|
| `hostname -I`             | Show your local IP address                 |
| `ping -c 1 google.com`    | Get IP address of google.com and test DNS  |
| `ping -c 1 8.8.8.8`       | Check if Internet works using Google DNS   |
| `which node`              | Find the location of the node command      |
| `which code`              | Find the location of the code command      |

---

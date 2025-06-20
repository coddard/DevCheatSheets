# 🐧 Linux Commands Cheatsheet  
*A comprehensive reference guide for essential Linux commands*  

---

## 🛟 Terminal Basics: Getting Help  

| Command              | Description                        | Example         |
|----------------------|------------------------------------|-----------------|
| `man <command>`      | Manual page for the command        | `man ls`        |
| `command --help`     | Short help for a command           | `rm --help`     |
| `help <builtin>`     | Help for shell built-in commands   | `help cd`       |
| `type <command>`     | Type of command (builtin/file)     | `type rm`       |
| `man -k <keyword>`   | Search keyword in man pages        | `man -k uname`  |
| `apropos <keyword>`  | Search for keyword in all man pages| `apropos passwd`|

---

## ⌨️ Keyboard Shortcuts  

| Shortcut          | Description                     |
|-------------------|---------------------------------|
| `TAB TAB`         | Show possible completions       |
| `CTRL + L`        | Clear terminal screen          |
| `CTRL + D`        | Logout/Close shell             |
| `CTRL + U`        | Cut current line               |
| `CTRL + A`        | Go to beginning of line        |
| `CTRL + E`        | Go to end of line              |
| `CTRL + C`        | Terminate current process      |
| `CTRL + Z`        | Suspend current process        |
| `CTRL + ALT + T`  | Open a new terminal window     |

---

## 🕰️ Bash History  

| Command                     | Description                                |
|-----------------------------|--------------------------------------------|
| `history`                   | Show history of executed commands          |
| `history -d <line>`         | Delete a line from history                 |
| `history -c`                | Clear all history                          |
| `!!`                        | Rerun last command                         |
| `!<n>`                      | Rerun nth command                          |
| `!<string>`                 | Run last command starting with string      |
| `!<string>:p`               | Print, don’t execute the command           |
| `CTRL + R`                  | Reverse search in history                  |
| `echo $HISTSIZE`            | Number of stored commands                 |
| `HISTTIMEFORMAT="..."`      | Show timestamps (add to `.bashrc`)         |

---

## 🔑 Root Access & User Passwords  

| Command                | Description                          |
|------------------------|--------------------------------------|
| `sudo <command>`       | Run command with root privileges     |
| `sudo su`              | Become root temporarily              |
| `su`                   | Switch to root user                  |
| `sudo passwd root`     | Set/change root password             |
| `passwd <username>`    | Change password for user             |

---

## 📁 Path & Directory Navigation  

| Command            | Description                     |
|--------------------|---------------------------------|
| `pwd`              | Show current directory          |
| `cd` / `cd ~`      | Go to home directory            |
| `cd -`             | Return to previous directory    |
| `cd /path/to/dir`  | Change to specific directory    |
| `.`                | Current directory               |
| `..`               | Parent directory                |
| `~`                | Home directory                  |

---

## 📦 Installing & Using Tools  

| Command               | Description                             |
|-----------------------|-----------------------------------------|
| `sudo apt install`    | Install package (Debian/Ubuntu)         |
| `tree .`              | Show directory structure                |
| `tree -d .`           | Show only directories                   |
| `tree -f .`           | Show full path names                    |

---

## 📋 Viewing Directories (ls)  

| Command         | Description                     |
|-----------------|---------------------------------|
| `ls`, `ls .`    | List current directory          |
| `ls ~ /var /`   | List multiple dirs              |
| `ls -l`         | Long listing format             |
| `ls -a`         | Show hidden files               |
| `ls -lh`        | Human-readable sizes            |
| `ls -lt`        | Sort by modification time       |
| `ls -i`         | Show inode numbers              |

---

## 📊 Disk Usage & Timestamps  

| Command          | Description                         |
|------------------|-------------------------------------|
| `du -sh ~`       | Disk usage of home dir              |
| `ls -lu`         | Access time                         |
| `ls -lc`         | Change time                         |
| `stat <file>`    | Show all timestamps                 |
| `touch <file>`   | Update/create file timestamp        |
| `date`           | Show current date/time              |
| `cal`            | Show calendar                       |

---

## 📄 Viewing Files  

| Command               | Description                         |
|-----------------------|-------------------------------------|
| `cat <file>`          | Show file contents                  |
| `cat -n <file>`       | Show with line numbers              |
| `less`, `more`        | View files with navigation          |
| `head <file>`         | Show first 10 lines                 |
| `tail <file>`         | Show last 10 lines                  |
| `watch -n 3 ls -l`    | Refresh every 3 seconds             |

---

## 🗃️ File/Directory Management  

| Command             | Description                   |
|---------------------|-------------------------------|
| `touch file`        | Create/update file            |
| `mkdir dir`         | Create directory              |
| `cp file1 file2`    | Copy file                     |
| `mv file1 file2`    | Rename/move file              |
| `rm file`           | Delete file                   |
| `rm -rf dir`        | Force remove directory        |
| `shred -vu file`    | Secure delete                 |

---

## 🔀 Piping & Redirection  

| Operator    | Description                         |
|-------------|-------------------------------------|
| `|`         | Pipe output to another command     |
| `>`         | Redirect stdout to file            |
| `>>`        | Append stdout to file              |
| `2>`        | Redirect stderr                    |
| `2>&1`      | Combine stderr and stdout          |

---

## 🔍 Finding Files  

| Command                     | Description                     |
|-----------------------------|---------------------------------|
| `locate <name>`             | Find by name (DB-based)         |
| `find ~ -type f -size +1M`  | Find large files                |
| `which <command>`           | Show executable path            |

---

## 🐧 grep: Search Text  

| Option   | Description                     |
|----------|---------------------------------|
| `-n`     | Show line number                |
| `-i`     | Case insensitive                |
| `-v`     | Invert match                    |
| `-w`     | Match whole word                |
| `-c`     | Count matches                   |
| `-R`     | Recursive search                |
| `-C 3`   | Show context (3 lines)          |

---

## ✏️ Text Editing with VIM  

| Command       | Description                     |
|---------------|---------------------------------|
| `vim file`    | Open file in vim                |
| `:wq!`        | Save and quit                   |
| `x` / `dd`    | Delete character/line           |
| `/string`     | Search forward                  |
| `?string`     | Search backward                 |
| `:e!`         | Reload file                     |

---

## 👥 User & Group Management  

| Command                     | Description               |
|-----------------------------|---------------------------|
| `useradd`, `userdel`        | Add/Delete user           |
| `usermod`                   | Modify user               |
| `groupadd`, `groupdel`      | Add/Delete group          |
| `who`, `id`, `w`            | Show user/system info     |

---

## 🔐 File Permissions & Ownership  

| Command               | Description                     |
|-----------------------|---------------------------------|
| `ls -l`               | View permissions                |
| `chmod u+x file`      | Add execute to user             |
| `chmod 755 file`      | Numeric permissions             |
| `chown user file`     | Change owner                   |
| `chgrp group file`    | Change group                   |

---

## 📈 Process Management  

| Command               | Description                 |
|-----------------------|-----------------------------|
| `ps -ef`, `top`, `htop` | View processes            |
| `kill <PID>`          | Kill process                |
| `killall <name>`      | Kill by name               |
| `jobs`, `fg`, `bg`    | Job control                |

---

## 🌐 Networking Basics  

| Command                     | Description                 |
|-----------------------------|-----------------------------|
| `ifconfig`, `ip a`          | Show interfaces             |
| `ip link set <dev> up/down` | Enable/disable interface    |
| `ip route`                  | Routing table               |
| `ping`, `traceroute`, `dig` | Network utilities          |

---

## 🔒 SSH & SCP  

| Command                 | Description                 |
|-------------------------|-----------------------------|
| `ssh user@host`         | Connect via SSH             |
| `scp file user@host:`   | Copy to remote              |
| `rsync -av /src /dest`  | Efficient sync              |

---

## 📡 Network Monitoring  

| Command         | Description                 |
|-----------------|-----------------------------|
| `netstat`, `ss` | Show connections            |
| `lsof -i`       | Open files/network          |
| `nmap`          | Network scanning            |

---

## 📦 Package Management (APT & DPKG)  

| Command                  | Description               |
|--------------------------|---------------------------|
| `sudo apt update`        | Update package list       |
| `sudo apt install <pkg>` | Install package           |
| `sudo apt remove <pkg>`  | Remove package            |
| `dpkg -i <file.deb>`     | Install local .deb        |
| `dpkg -L <pkg>`          | List files in package     |

---

## ⏰ Cron Jobs  

| Format        | Description       |
|---------------|-------------------|
| `* * * * *`   | Every minute      |
| `@daily`      | Every day         |
| `@reboot`     | At boot           |
| `crontab -e`  | Edit jobs         |
| `crontab -l`  | List jobs         |

---

## 💻 Hardware Info  

| Command               | Description             |
|-----------------------|-------------------------|
| `lscpu`, `lshw`, `lsblk` | CPU/HW/disk info      |
| `free -m`             | Memory usage            |
| `lsusb`, `lspci`      | USB & PCI devices       |
| `uname -a`            | Kernel/system info      |

---

## ⚙️ Device & Systemd Services  

| Command                 | Description             |
|-------------------------|-------------------------|
| `dd`                    | Clone/backup disks      |
| `systemctl status <svc>`| Show service status     |
| `systemctl start/stop`  | Control services        |
| `systemd-analyze`       | Boot performance        |

---

## 📜 Bash Scripting Essentials  

| Concept           | Example                              |
|-------------------|--------------------------------------|
| Define Variable   | `x=5`                                |
| If Condition      | `if [ $x -gt 3 ]; then echo OK; fi`  |
| Loops             | `for i in {1..5}; do echo $i; done`  |
| Functions         | `myfunc() { echo Hello; }`           |
| Aliases           | `alias ll='ls -lah'`                 |

# 🐧 Linux Commands Cheatsheet  

---

### 🧰 Terminal Basics  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `📚` | `man <command>` | View manual pages (navigate with `q` to quit) |  
| `🔍` | `type <command>` | Check if command is built-in or executable |  
| `💡` | `help <command>` | Get help for shell built-ins |  
| `📜` | `man -k <keyword>` | Search man pages (e.g., `man -k copy`) |  

---

### 📁 File & Directory Navigation  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `📂` | `pwd` | Print current directory |  
| `🧭` | `cd <path>` | Change directory (`cd ~` for home, `cd -` for last dir) |  
| `📋` | `ls` | List files (`ls -la` for hidden files, `ls -lh` for human-readable sizes) |  
| `📊` | `du -sh <dir>` | Show directory size |  

---

### 🔧 File Operations  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `📄` | `touch <file>` | Create a new file |  
| `🗂️` | `mkdir <dir>` | Create a directory (`mkdir -p nested/dirs` for nested dirs) |  
| `📋` | `cp <src> <dest>` | Copy files (`cp -r` for directories) |  
| `✂️` | `mv <src> <dest>` | Move/rename files |  
| `🗑️` | `rm <file>` | Delete files (`rm -rf` for force delete) |  

---

### 🔍 Searching & Text Manipulation  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `🔎` | `grep "pattern" <file>` | Search text (`grep -r` for recursive, `grep -i` for case-insensitive) |  
| `📄` | `cat <file>` | Display file contents |  
| `📄` | `less <file>` | Scrollable file viewer (`q` to quit) |  
| `📈` | `head/tail <file>` | View first/last lines (`tail -f` for real-time logs) |  

---

### 🧪 Processes  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `🚦` | `ps aux` | List all processes |  
| `🔍` | `pgrep <process>` | Find process by name |  
| `🛑` | `kill <PID>` | Kill a process (`kill -9` for force kill) |  
| `⏱️` | `top` / `htop` | Real-time process monitor |  
| `🔌` | `nohup <command>` | Run process immune to hangups |  

---

### 🌐 Networking  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `📡` | `ifconfig` / `ip addr` | Check IP addresses |  
| `🌐` | `ping <host>` | Test connectivity |  
| `🔗` | `ssh user@host` | Secure shell login (`ssh -p <port>` for custom ports) |  
| `📥` | `scp <src> <dest>` | Secure file copy (`scp -r` for directories) |  
| `🌍` | `wget <url>` | Download files |  

---

### 🔐 Permissions  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `🔐` | `chmod <permissions> <file>` | Change file permissions (`chmod 755 file`) |  
| `👤` | `chown <user>:<group> <file>` | Change owner/group |  
| `🛡️` | `sudo <command>` | Execute as root |  
| `🔑` | `su` | Switch to root user |  

---

### ⚙️ System Info  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `🧠` | `uname -a` | System info |  
| `💾` | `df -h` | Disk usage |  
| `🔋` | `acpi -bi` | Battery status |  
| `📡` | `lshw` | Hardware details |  

---

### 🧰 Advanced Tools  

| Emoji | Command | Description |  
|-------|---------|-------------|  
| `🔁` | `rsync -av <src> <dest>` | Sync files/dirs |  
| `📦` | `tar -czvf <file.tar.gz> <dir>` | Compress files (`-x` to extract) |  
| `🧼` | `shred -vu <file>` | Securely delete files |  
| `🔍` | `locate <file>` | Fast file search (requires `updatedb`) |  
| `🔍` | `find <path> -name "<pattern>"` | Powerful file search |  

---

### 💡 Final Tips  

| Emoji | Tip |  
|-------|-----|  
| `⌨️` | Use `TAB` for auto-complete, `CTRL+C` to cancel |  
| `📜` | `history` shows command history (`!20` re-runs command #20) |  
| `⚡` | Combine commands with `|` (pipe): `ps aux | grep ssh` |  
| `🔄` | Schedule tasks with `crontab -e` (e.g., `0 3 * * * backup_script.sh`) |  
| `🪄` | Use aliases: `alias ll='ls -la'` |  

---

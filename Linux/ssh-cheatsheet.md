
### 🚀 Ultimate SSH/SCP/SFTP Cheat Sheet

Your Swiss Army Knife for Secure Remote Operations! 🔐💻

---

# 🚀 Ultimate SSH/SCP/SFTP Cheat Sheet  
**Your Swiss Army Knife for Secure Remote Operations!** 🔐💻  

---

## 🔌 Basic SSH Connections

| Command | Description | Emoji |
|--------|-------------|-------|
| `ssh user@host` | Connect to host on port 22 | 🌐➡️💻 |
| `ssh -p 2222 user@host` | Custom port connection | 🔢🚪 |
| `ssh -i ~/.ssh/aws.pem ubuntu@ec2-ip` | Use private key for authentication | 🔑🔓 |
| `ssh -v user@host` | Verbose output (for debugging) | 🐞🔍 |
| `ssh -o "StrictHostKeyChecking=no" host` | Skip host verification | ⚠️🚨 |
| `ssh -o "ConnectTimeout=5" host` | Set timeout for connection attempt | ⏱️🚫 |
| `mosh user@host` | Mobile shell for unstable connections | 📱✨ |
| `ssh -t user@host sudo su -` | Force pseudo-terminal allocation | 🖥️🔑 |
| `ssh -q user@host` | Quiet mode (suppress banner messages) | 🤫 |
| `ssh -T git@github.com` | Test GitHub connectivity | 🧪🌐 |

---

## 🔑 SSH Key Management

| Command | Description | Emoji |
|--------|-------------|-------|
| `ssh-keygen -t ed25519 -a 100 -C "work@email"` | Generate modern Ed25519 key | 🔐 |
| `ssh-keygen -t rsa -b 4096 -f ~/.ssh/backup_key` | Generate RSA fallback key | 🔒 |
| `ssh-copy-id -i ~/.ssh/id_ed25519.pub -p 2222 user@host` | Copy public key to server | 📤 |
| `ssh-keygen -l -f ~/.ssh/id_ed25519` | List fingerprint of a key | 🖐️🔢 |
| `ssh-add ~/.ssh/*` | Add all keys to agent | 👨‍💼 |

---

## 📁 File Transfers

### SCP (Secure Copy)

| Command | Description | Emoji |
|--------|-------------|-------|
| `scp -rpC -P 2222 ~/projects user@host:/backups/` | Compressed recursive copy | 📦 |
| `scp -3 user1@host1:/file user2@host2:/dir` | Transfer between two remote hosts | 🔄 |

### SFTP (Interactive File Transfer)

| Command | Description | Emoji |
|--------|-------------|-------|
| `sftp -P 2222 user@host` | Connect to remote via SFTP | 📲 |
| `put -r local_dir` | Upload directory recursively | 📤📁 |
| `get -r remote_dir` | Download directory recursively | 📥📁 |
| `chmod 600 file` | Change permissions remotely | 🔧 |

### rsync (Advanced Sync)

| Command | Description | Emoji |
|--------|-------------|-------|
| `rsync -azP -e "ssh -p 2222" --delete --exclude='*.tmp' ~/docs/ user@host:/backups/` | Mirror with exclusions | 🔄🗑️ |
| `rsync -azP --partial ~/large.iso user@host:/iso/` | Resume partial transfers | 🛠️⏳ |

---

## ⚙️ SSH Configuration Magic

### Example: `~/.ssh/config`
```text
Host myserver
  HostName server.com
  User admin
  Port 2222
  IdentityFile ~/.ssh/server_key
  Compression yes
  ServerAliveInterval 60

Host *.internal
  ProxyJump bastion
  User dev

Host github.com
  User git
  IdentityFile ~/.ssh/github_key
  IdentitiesOnly yes
```

| Feature | Description | Emoji |
|--------|-------------|-------|
| `ProxyJump bastion` | Jump through a bastion host | 🧭 |
| `ControlMaster auto` | Reuse existing SSH connections | 🧵 |
| `ControlPath ~/.ssh/cm_socket/%r@%h:%p` | Socket path for multiplexing | 🧬 |
| `ControlPersist 4h` | Keep master connection open | ⏳ |

---

## 🛠️ Advanced SSH Features

| Command | Description | Emoji |
|--------|-------------|-------|
| `ssh -fNMS ~/.ssh/mux_socket myserver` | Start multiplex master | 🧵 |
| `ssh -S ~/.ssh/mux_socket myserver` | Reuse existing session | 🚀 |
| `ssh -L 3306:db.internal:3306 bastion` | Local port forwarding (MySQL tunnel) | 🔁 |
| `ssh -R 8080:localhost:80 public` | Remote port forwarding | 🔁🌍 |
| `ssh -D 1080 proxy` | Dynamic SOCKS proxy | 🧙‍♂️🌐 |
| `ssh -X user@host` | Forward X11 GUI apps | 🎨🖥️ |
| `ssh -J admin@bastion user@internal` | Inline jump host command | 🧭 |
| `ssh user@host "echo ok"` | Run command on remote | 💬🖥️ |
| `ssh -o BatchMode=yes user@host "uptime"` | No password prompts | 🤖 |

---

## 🔒 Security Hardening

| Config Directive | Description | Emoji |
|------------------|-------------|-------|
| `Port 2222` | Change default port | 🔢 |
| `PermitRootLogin no` | Disable root login | 🚫👑 |
| `PasswordAuthentication no` | Keys only | 🔑🔒 |
| `AllowUsers admin deploy` | Whitelist users | ✅👥 |
| `MaxAuthTries 3` | Prevent brute force | 🛡️ |
| `ClientAliveInterval 300` | Disconnect idle sessions | ⏳ |

| Command | Description | Emoji |
|--------|-------------|-------|
| `sudo systemctl reload sshd` | Reload config without restart | 🔄 |
| `sudo journalctl -u sshd -f` | View live logs | 📜🔍 |
| `sudo last -i` | Check recent logins | 📋✅ |

---

## 🚨 Troubleshooting & Diagnostics

| Command | Description | Emoji |
|--------|-------------|-------|
| `ssh -vvv user@host` | Debugging output | 🐞🔍 |
| `nc -zv host 2222` | Check if port is open | 🕵️‍♂️ |
| `ss -tnpa \| grep ssh` | Show active SSH sessions | 📡 |
| `chmod 700 ~/.ssh && chmod 600 ~/.ssh/*` | Fix permission issues | 🔧 |

| Escape Sequence | Description | Inside SSH Session |
|------------------|-------------|--------------------|
| `Enter` then `~?` | Show escape help | ✨ |
| `~.` | Terminate connection | ❌ |
| `~^Z` | Background session | ⏸️ |
| `~C` | Open SSH command line (add port forwards) | 🧰 |

---

## 📚 Recommended Tools

| Tool | Purpose | Install Command |
|------|---------|-----------------|
| `autossh` | Auto-reconnect tunnels | `apt install autossh` |
| `tmux` | Persistent sessions | `apt install tmux` |
| `ngrok` | Public tunnels | [ngrok.com](https://ngrok.com) |
| `sshfs` | Mount remote FS | `apt install sshfs` |
| `netcat` | Network debugging | `apt install netcat` |

---

## 🎯 Pro Tips

- **Modern Keys**: Prefer `ed25519` over RSA for better performance/security
- **Key Passphrases**: Use `ssh-agent` to avoid re-entering them every time
- **Config Files**: Master `~/.ssh/config` to simplify complex setups
- **Persistent Tunnels**: Use `autossh` for reliable port forwards
- **File Transfer**: Prefer `rsync` over `scp` for large syncs
- **Security**: Always disable password auth in production
- **MFA**: Add 2FA using `google-authenticator` for critical servers
- **Algorithms**: Use `ssh -Q cipher/mac/kex/key` to check supported options

---

## 💡 Fun Fact  
SSH can tunnel any TCP traffic – databases, VNC, even games! 🎮⚡  

---

## 🐚 Happy Secure Shell-ing!  
Stay safe out there! 🔒🛡️  

---




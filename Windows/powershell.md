# 🐚 PowerShell Cheat Sheet

**A colorful guide to PowerShell commands for sysadmins and DevOps engineers 🌟**

---

## 📁 File Management

| Emoji | Command                                    | Description                    |
| ----- | ------------------------------------------ | ------------------------------ |
| 📋    | `Get-ChildItem`                            | List files and directories     |
| 📄    | `Get-Content <file>`                       | Get content of a file          |
| ✏️    | `Set-Content <file> <content>`             | Set content of a file          |
| 📄    | `New-Item <file>`                          | Create a new file              |
| 📁    | `New-Item <directory> -ItemType Directory` | Create a new directory         |
| 🗑️    | `Remove-Item <file>`                       | Remove a file                  |
| 🗑️    | `Remove-Item <directory> -Recurse`         | Remove a directory (recursive) |
| 🔄    | `Rename-Item <file> <new_file>`            | Rename a file or directory     |
| 📤    | `Copy-Item SOURCE DEST`                    | Copy a file                    |
| 📤    | `Copy-Item SOURCE DEST -Recurse`           | Copy a directory               |
| 📥    | `Move-Item SOURCE DEST`                    | Move a file or directory       |

---

## 🏃 Process Management

| Emoji | Command                        | Description                  |
| ----- | ------------------------------ | ---------------------------- |
| 📋    | `Get-Process`                  | List running processes       |
| ⏹️    | `Stop-Process -Name <process>` | Stop a process               |
| 🚀    | `Start-Process <process>`      | Start a new process          |
| ⏳    | `Wait-Process -Name <process>` | Wait for a process to finish |

---

## ⚙️ Service Management

| Emoji | Command                                        | Description                 |
| ----- | ---------------------------------------------- | --------------------------- |
| 📋    | `Get-Service`                                  | List services               |
| ▶️    | `Start-Service <service>`                      | Start a service             |
| ⏹️    | `Stop-Service <service>`                       | Stop a service              |
| 🔁    | `Restart-Service <service>`                    | Restart a service           |
| 🔄    | `Set-Service <service> -StartupType Automatic` | Set service to auto-start   |
| 🔄    | `Set-Service <service> -StartupType Manual`    | Set service to manual start |
| 🚫    | `Set-Service <service> -StartupType Disabled`  | Disable a service           |

---

## 👤 User Management

| Emoji | Command                                                        | Description                  |
| ----- | -------------------------------------------------------------- | ---------------------------- |
| 👥    | `Get-LocalUser`                                                | List local users             |
| 🆕    | `New-LocalUser <user>`                                         | Create a new local user      |
| 🗑️    | `Remove-LocalUser <user>`                                      | Remove a local user          |
| 🔒    | `Set-LocalUser <user> -Password <password>`                    | Set user password            |
| 👨‍💻    | `Add-LocalGroupMember -Group Administrators -Member <user>`    | Add user to Admin group      |
| 🚫    | `Remove-LocalGroupMember -Group Administrators -Member <user>` | Remove user from Admin group |

---

## 🌐 Network Management

| Emoji | Command            | Description           |
| ----- | ------------------ | --------------------- |
| 🌐    | `Get-NetIPAddress` | List IP addresses     |
| 🖥️    | `Get-NetAdapter`   | List network adapters |

---

## 🧩 Windows Updates

| Emoji | Command                                | Description                    |
| ----- | -------------------------------------- | ------------------------------ |
| 📦    | `Install-Module -Name PSWindowsUpdate` | Install PSWindowsUpdate module |
| 📋    | `Get-Command -Module PSWindowsUpdate`  | List commands in module        |
| 🔄    | `Get-WUInstall`                        | Install Windows updates        |

---

## 🧰 Windows Features

| Emoji | Command                              | Description                 |
| ----- | ------------------------------------ | --------------------------- |
| 📋    | `Get-WindowsFeature`                 | List Windows features       |
| 🆕    | `Install-WindowsFeature <feature>`   | Install a Windows feature   |
| 🗑️    | `Uninstall-WindowsFeature <feature>` | Uninstall a Windows feature |

---

## 🌐 Remote Connection

| Emoji | Command                                                          | Description                    |
| ----- | ---------------------------------------------------------------- | ------------------------------ |
| 💻    | `Enter-PSSession -ComputerName <name> -Credential <user>`        | Open remote session            |
| 🚪    | `Exit-PSSession`                                                 | Close current remote session   |
| 📡    | `Invoke-Command -ComputerName <name> -ScriptBlock { <command> }` | Run command on remote computer |
| 📡    | `Invoke-Command -ComputerName <name> -FilePath <script>`         | Run script on remote computer  |

---

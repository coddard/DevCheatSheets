# 🍺 Homebrew Cheat Sheet

**Your one-stop shop for macOS package management magic!**

---

## 📚 Table of Contents

1. [📦 Getting Started](#getting-started)
2. [🔍 Commands](#commands)
3. [🔧 Help & Diagnostics](#help--diagnostics)
4. [🔄 Update Management](#update-management)
5. [🔌 Taps & Repositories](#taps--repositories)
6. [💾 Cask Applications](#cask-applications)
7. [🔍 Search & Info](#search--info)
8. [📥 Install & Uninstall](#install--uninstall)
9. [🧹 Cleanup](#cleanup)
10. 💡 Pro Tips

---

## 📦 Getting Started

**Install Homebrew** (if not already installed):

```bash
# Install Command Line Tools (CLT)
xcode-select --install

# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

🔗 [Official Website](https://brew.sh/)

---

## 🔍 Commands

| Emoji | Command                    | Description             |
| ----- | -------------------------- | ----------------------- |
| 📦    | `brew install git`         | Install a package       |
| 🧹    | `brew uninstall git`       | Uninstall a package     |
| 🔁    | `brew upgrade git`         | Upgrade package         |
| 🔗    | `brew link git`            | Link package            |
| 🚫    | `brew unlink git`          | Unlink package          |
| 🔄    | `brew switch git 1.0.0`    | Switch package version  |
| 📋    | `brew list --versions git` | List installed versions |

---

## 🔧 Help & Diagnostics

| Emoji | Command          | Description             |
| ----- | ---------------- | ----------------------- |
| ℹ️    | `brew --version` | Show Homebrew version   |
| ❓    | `brew help`      | Print help info         |
| 🛠️    | `brew doctor`    | Check for system issues |

---

## 🔄 Update Management

| Emoji | Command                  | Description                    |
| ----- | ------------------------ | ------------------------------ |
| 🔄    | `brew update`            | Fetch latest Homebrew updates  |
| 📉    | `brew outdated`          | Show outdated packages         |
| 🚀    | `brew upgrade`           | Upgrade all outdated packages  |
| 🚀    | `brew upgrade <formula>` | Upgrade specific package       |
| 🛑    | `brew pin <formula>`     | Prevent package from upgrading |
| 🔄    | `brew unpin <formula>`   | Allow package to upgrade       |

---

## 🔌 Taps & Repositories

| Emoji | Command                      | Description                  |
| ----- | ---------------------------- | ---------------------------- |
| 📂    | `brew tap`                   | List all tapped repositories |
| 📥    | `brew tap <user/repo>`       | Tap a GitHub repo            |
| 📥    | `brew tap <user/repo> <URL>` | Tap a custom URL repo        |
| 🗑️    | `brew untap <user/repo>`     | Remove a tap                 |

---

## 💾 Cask Applications

| Emoji | Command                     | Description              |
| ----- | --------------------------- | ------------------------ |
| 📦    | `brew tap homebrew/cask`    | Tap Cask repository      |
| 📋    | `brew cask list`            | List installed Cask apps |
| 🔍    | `brew search <text>`        | Search Cask apps         |
| 🚀    | `brew cask install <app>`   | Install Cask app         |
| 🔁    | `brew cask reinstall <app>` | Reinstall Cask app       |
| 🧹    | `brew cask uninstall <app>` | Uninstall Cask app       |

---

## 🔍 Search & Info

| Emoji | Command               | Description          |
| ----- | --------------------- | -------------------- |
| 🔍    | `brew search`         | Search formulae      |
| 🔍    | `brew search <text>`  | Search by keyword    |
| ℹ️    | `brew info <formula>` | Show package details |

---

## 📥 Install & Uninstall

| Emoji | Command                    | Description       |
| ----- | -------------------------- | ----------------- |
| 📦    | `brew install <formula>`   | Install package   |
| 🧹    | `brew uninstall <formula>` | Uninstall package |

---

## 🧹 Cleanup

| Emoji | Command                  | Description                          |
| ----- | ------------------------ | ------------------------------------ |
| 🧹    | `brew cleanup`           | Remove old package versions          |
| 🧹    | `brew cleanup <formula>` | Clean specific package               |
| 🔍    | `brew cleanup -n`        | Dry run (show what would be cleaned) |

---

## 💡 Pro Tips

- 🧠 **Batch operations**:
  ```bash
  # Install multiple packages
  brew install git curl wget
  ```
- 🧩 **Custom taps**: Use `brew tap` to add third-party repositories.
- 📦 **Cask apps**: Install GUI apps like VSCode with `brew install --cask visual-studio-code`.
- 🔄 **Update strategy**: Run `brew update && brew upgrade` weekly to stay current.

---

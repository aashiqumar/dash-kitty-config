# 🐱 Kitty Terminal Configuration

<img width="1920" alt="Migration Dashboard Screenshot" src="https://github.com/user-attachments/assets/46de2405-001e-435a-abe8-32f9a775ae68" />

A high-performance, GPU-accelerated terminal environment optimized for **Oracle/MongoDB migrations** and full-stack development. This setup features a custom 3-pane layout, **Catppuccin Mocha** aesthetics, and frosted glass transparency.

## 🚀 Installation

### 1. Install Kitty
On Ubuntu, use the official repository to ensure the package is managed by `apt`.
```bash
sudo apt update && sudo apt install kitty -y

# 🛠️ Configuration Steps

Follow these steps to apply the custom "Migration Dashboard" theme to your local machine.

## 1. Directory Setup
Before linking your files, ensure the Kitty configuration directory exists in your home folder.
```bash
mkdir -p ~/.config/kitty

2. Linking Dotfiles

Instead of copying files, use a symbolic link. This ensures that any changes you make in your GitHub repository folder are automatically applied to your system.

    Note: Replace ~/projects/migration-dash-kitty with the actual path where you cloned the repository.

Bash

# Remove existing config if it exists
rm -rf ~/.config/kitty/kitty.conf

# Create the symbolic link
ln -sf ~/projects/migration-dash-kitty/kitty.conf ~/.config/kitty/kitty.conf

3. Applying the Theme

If your configuration uses an external theme file (like current-theme.conf for Catppuccin), ensure it is also linked or present in the same directory.
Bash

ln -sf ~/projects/migration-dash-kitty/current-theme.conf ~/.config/kitty/current-theme.conf

4. Verification & Reload

You do not need to restart your computer or the terminal to see changes. Use Kitty's built-in reload command to refresh the UI instantly.

    Focus your Kitty terminal.

    Press Ctrl + Shift + F5.

    If the white title bar is still visible, ensure hide_window_decorations yes is set in your config and restart the app once.


## ⌨️ Essential Keyboard Shortcuts

These mappings are optimized for a high-performance workflow, ensuring no conflicts with standard system commands like **Copy** (`Ctrl+Shift+C`) and **Paste** (`Ctrl+Shift+V`).

### 🪟 Window & Pane Management (Splits)
| Shortcut | Action |
| :--- | :--- |
| `Ctrl` + `Shift` + `S` | **Horizontal Split** (Create pane below) |
| `Ctrl` + `Shift` + `D` | **Vertical Split** (Create pane to the right) |
| `Ctrl` + `Shift` + `Enter` | **Quick Horizontal Split** (Follows current path) |
| `Ctrl` + `Shift` + `Q` | **Close Focused Pane** (Terminates current session) |
| `Ctrl` + `Shift` + `Z` | **Toggle Zoom** (Maximize active pane to full screen) |

### 🎯 Navigation & Focus
| Shortcut | Action |
| :--- | :--- |
| `Ctrl` + `Shift` + `H` | Move focus to the **Left** pane |
| `Ctrl` + `Shift` + `L` | Move focus to the **Right** pane |
| `Ctrl` + `Shift` + `K` | Move focus to the **Upper** pane |
| `Ctrl` + `Shift` + `J` | Move focus to the **Lower** pane |

### 📏 Resizing Panes
| Shortcut | Action |
| :--- | :--- |
| `Ctrl` + `Left Arrow` | Make focused pane **Narrower** |
| `Ctrl` + `Right Arrow` | Make focused pane **Wider** |
| `Ctrl` + `Up Arrow` | Make focused pane **Taller** |
| `Ctrl` + `Down Arrow` | Make focused pane **Shorter** |
| `Ctrl` + `Home` | **Reset** all panes to equal size |

### ⚙️ System & Tabs
| Shortcut | Action |
| :--- | :--- |
| `Ctrl` + `Alt` + `Tab` | Switch to **Next Tab** |
| `Ctrl` + `Shift` + `Alt` + `Tab` | Switch to **Previous Tab** |
| `Ctrl` + `Shift` + `F5` | **Reload Configuration** (Apply changes live) |
| `Ctrl` + `Shift` + `F2` | **Edit kitty.conf** in default text editor |


🐱 Kitty Terminal Configuration

<img width="1920" height="1173" alt="Screenshot from 2026-02-11 16-14-59" src="https://github.com/user-attachments/assets/46de2405-001e-435a-abe8-32f9a775ae68" />


A high-performance, GPU-accelerated terminal environment optimized for Oracle/MongoDB migrations and full-stack development. This setup features a custom 3-pane layout, Catppuccin Mocha aesthetics, and frosted glass transparency.
🚀 Installation
1. Install Kitty

On Ubuntu, use the official repository to ensure the package is managed by apt.
Bash

sudo apt update && sudo apt install kitty -y

2. Set as Default Terminal (Optional)

To make Kitty your system default:
Bash

sudo update-alternatives --config x-terminal-emulator

🛠️ Configuration
1. Apply Custom Dotfiles

Link your kitty.conf from your repository to the standard Kitty configuration path.
Bash

# Create the directory if it doesn't exist
mkdir -p ~/.config/kitty

# Create a symbolic link to your custom config
ln -sf ~/path/to/your/repo/kitty.conf ~/.config/kitty/kitty.conf

2. Install Required Fonts

This configuration requires Monolisa Nerd Font and Maple Mono for proper rendering and italics. Ensure these are installed in ~/.local/share/fonts.
⌨️ Essential Keyboard Shortcuts

These mappings are optimized to avoid conflicts with system "Paste" (Ctrl+Shift+V) and "Copy" (Ctrl+Shift+C).
Window Management (Splits)
Command	Action
Ctrl + Shift + S	Split Horizontally (Pane below)
Ctrl + Shift + D	Split Vertically (Pane to the right)
Ctrl + Shift + Q	Close Current Pane
Ctrl + Shift + Z	Toggle Zoom (Stack/Unstack pane)
Navigation & Resizing
Command	Action
Ctrl + Shift + H/J/K/L	Move Focus (Vim-style Left/Down/Up/Right)
Ctrl + Arrow Keys	Resize Active Pane
Ctrl + Home	Reset All Pane Sizes
System Commands
Command	Action
Ctrl + Shift + F5	Reload Config (Live update)
Ctrl + Shift + F2	Edit Config in default editor
📊 Dashboard Setup (Recommended Commands)

To achieve the "Command Center" look for your migration monitoring, open three panes and run:

    Top Pane: Your Migration Script (python3 migrate.py).

    Bottom Left: btop for system telemetry.

    Bottom Right: docker stats for database health monitoring.

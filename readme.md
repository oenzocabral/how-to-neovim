# Neovim Tutorial: From Basics to Advanced

### Perfect for beginners starting with Vim/Neovim and experienced users looking to level up their skills.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Getting Started](#getting-started)
    - [Modes](#modes)
    - [Commands and Motions](#commands-and-motions)
    - [Basic Commands](#basic-commands)
4. [Advanced Topics](#advanced-topics)
5. [References](#references)

---

## Introduction
Neovim is a modern, highly extensible text editor based on Vim. It is loved for its speed, efficiency, and customizability. Whether you’re a developer, writer, or power user, Neovim can significantly enhance your productivity.

---

## Installation
Not covered in detail here, but you can check the [official Neovim installation guide](https://github.com/neovim/neovim/blob/master/INSTALL.md) for instructions.

---

## Getting Started

### Modes
Neovim operates with multiple modes, each serving a distinct purpose:

1. **Normal Mode**:
    - Default mode when you open Neovim.
    - Use for navigation and executing commands.
    - Enter by pressing **ESC**.

2. **Insert Mode**:
    - Allows text editing.
    - Enter by pressing **i** (or **a**, **o** for variations).
    - Exit by pressing **ESC**.

3. **Visual Mode**:
    - Enables text selection.
    - Enter by pressing **v** for character selection, **V** for line selection, or **Ctrl-v** for block selection.
    - Exit by pressing **ESC**.

4. **Command Mode**:
    - Execute file operations like save, quit, and more.
    - Enter by typing **:**.
    - Exit by pressing **ESC** or executing a command.

---

### Commands and Motions
Commands and motions work together to perform efficient text editing.

- **Command**: An action performed on text (e.g., delete, yank, change).
- **Motion**: Specifies where the command applies (e.g., word, line).
- **Count**: Repeats the motion/command a specified number of times.

**Examples:**
- `4k`: Move cursor up 4 lines.
- `6w`: Move cursor forward 6 words.
- `d4w`: Delete the next 4 words.
- `y2j`: Yank the current and next 2 lines.

Note: Command and Motions only work on Normal and Visual mode

---

### Basic Commands (For Visual Mode)
Here are essential commands for everyday use:

| Command       | Description                                                      |
|---------------|------------------------------------------------------------------|
| `dd`          | Delete the current line.                                         |
| `y`           | Yank (copy) the selected text.                                   |
| `p`           | Paste the selected text                                          |
| `c`           | Change the selected text (deletes and enters Insert mode).       |
| `U`           | Convert the selected text to uppercase.                          |
| `u`           | Convert the selected text to lowercase.                          |
| `>`           | Indent the selected text.                                        |
| `<`           | Un-indent the selected text.                                     |
| `=`           | Auto-indent the selected text.                                   |

---

### Basic Motions
| Motion        | Description                                                      |
|---------------|------------------------------------------------------------------|
| `k`           | Move cursor up one line.                                         |
| `j`           | Move cursor down one line.                                       |
| `h`           | Move cursor left one character.                                  |
| `l`           | Move cursor right one character.                                 |
| `w`           | Move to the beginning of the next word.                          |
| `b`           | Move to the beginning of the previous word.                      |

---

### Combining Commands and Motions
You can combine commands for a more efficient editing.

| Combination   | Description                                                      |
|---------------|------------------------------------------------------------------|
| `d4w`         | Delete the next 4 words.                                         |
| `c3w`         | Change the next 3 words.                                         |
| `>2j`         | Indent the current and next 2 lines.                             |
| `y5k`         | Yank the current line and 4 lines above.                         |

---

### Basic Commands (For Command Mode)
| Command       | Description                                                      |
|---------------|------------------------------------------------------------------|
| `:w`          | Save the current file.                                           |
| `:q`          | Exites neovim.                                                   |
| `wq` or `:x`  | Save the current file and exit Neovim.                           |
| `:q!`         | Quit without saving changes.                                     |
| `:e filename` | Open or edit a file (filename).                                  |
| `:r filename` | Insert the contents of another file in the current cursor position.|
| `saveas file` | Save the current buffer to a new file.                             |
| `:set opt`    | Set an option (e.g., :set number for line numbers).                |
| `:noh`        | Remove search highlight.                                           |
| `:/pattern`   | Search for a pattern.                                              |
| `:s/foo/bar/  | Replace `foo` with `bar` on the current line.                      |
| `:%s/foo/bar/ | Replace `foo` with `bar` in the whole file.                        |
| `:!cmd`       | Run an external shell command.                                     |
| `:help cmd`   | Get help on a specific command.


## Begginner Tips
Before moving on to the next topics, first try to master swithcing between all 4 modes, and try to get confortable with using motions and commands to navigate trought the file. Even tho it might seem boring, it is essential that you master the basics before moving on to the most advanced topics.

For those who prefer to learn trough video, here is a YouTube video by @ThePrimeagen that might help you get the basics.
[![Watch the video](https://img.youtube.com/X6AR2RMB5tE/0.jpg)](https://youtu.be/X6AR2RMB5tE?si=jSgOOSSsMyUH4727)


## Advanced Topics

### Configuration
- Customize Neovim by editing the `init.lua` (or `init.vim`) file.
- Examples of configurations include:
    - Setting up key mappings.
    - Adjusting color schemes.
    - Enabling relative line numbers.

### Plugins
- Extend Neovim’s functionality with plugins.
- Popular plugin managers include:
    - `packer.nvim`
    - `vim-plug`

### Useful Workflows
- Split Windows: `:vsplit` (vertical) or `:split` (horizontal).
- Tabs: Use `:tabnew` to create a new tab.
- Search and Replace: `:%s/old/new/g` (global replacement).

---

## References
### YouTube Links
- [The Primeagen’s Tutorials](https://www.youtube.com/user/ThePrimeagen)
- [Chris@Machine’s Neovim Series](https://www.youtube.com/c/ChrisAtMachine)

### Official Documentation
- [Neovim Docs](https://neovim.io/doc/user/)

### Articles
- [Beginner's Guide to Neovim](https://neovim.io/learn/)
- [Advanced Neovim Tips](https://neovim.io/tips/)

### Repositories
- [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim): A minimal Neovim configuration.
- [Awesome Neovim](https://github.com/rockerBOO/awesome-neovim): A curated list of Neovim plugins and resources.

---

This guide will be continually updated with more tips, workflows, and advanced techniques. Happy editing!








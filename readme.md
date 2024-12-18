# How to Neovim

This repository a guide that teaches the basics all the way up to the advanced topics of Neovim. It includes resources, articles, repositories, and detailed explanations for each topic. It is being developed to be begginer friendly, but still, include advanced topics for Neovim users with some experience.

Note: This repository is still in development.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Contributions](#contributions)
3. [Installation](#installation)
4. [Getting Started](#getting-started)
    - [Modes](#modes)
    - [Commands and Motions](#commands-and-motions)
    - [Basic Commands](#basic-commands)
5. [Advanced Topics](#advanced-topics)
6. [References](#references)

---

## Introduction
Neovim is a modern, highly extensible text editor based on Vim. It is loved for its speed, efficiency, and customizability. Whether you’re a developer, writer, or power user, Neovim can significantly enhance your productivity.

---

## Contributions

We welcome contributions from everyone! If you have more experience with Neovim or if you simply have a better way to explain a concept, feel free to fork this repository and improve the content. You can contribute by updating the `README.md` file, adding new tutorials, or clarifying existing ones.

### How to Contribute:
1. Fork this repository.
2. Make your changes (feel free to improve explanations, add examples, or suggest new topics).
3. Submit a pull request with your changes.

Your contributions help make this repository better for everyone.

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

[![Watch the video](https://img.youtube.com/vi/X6AR2RMB5tE/0.jpg)](https://youtu.be/X6AR2RMB5tE?si=Q4khlOfHzkA_i5VB)


## More Motions
| Command       | Description                                                   |
|---------------|---------------------------------------------------------------|
| `_`           | Go to the begginning of the line.                     |
| `$`           | Go to the end of the line.                            |
| `0`           | Go to the initial character of the line (inluding indentation). |
| `f+character` | Go forward to the closest "character" to the cursor.  |
| `F+character` | Go backwards to the closes "character" to the cursor. |
| `t+character` | Go forward to the left of the specified character (not on the character). |
| `T+character` | Go backwards to the right of the specified character (not on the character). |
| `;`           | Repeat the action of `f` or `t` forward.    |
| `,`           | Repeat the action of `f` or `t` backwards.  |
| `I`           | Go to the beggining of the line in Insert Mode. |
| `A`           | Go to the end of the line in Insert Mode.        |
| `o`           | Create a new line under the cursor and go into Insert Mode. |
| `O`           | Create a new line above the cursor and go into Insert Mode. |


## References
### YouTube Links
- [The Primeagen’s Tutorials](https://www.youtube.com/watch?v=X6AR2RMB5tE&list=PLm323Lc7iSW_wuxqmKx_xxNtJC_hJbQ7R)
- [Chris@Machine’s Neovim Series](https://www.youtube.com/c/ChrisAtMachine)

### Official Documentation
- [Neovim Docs](https://neovim.io/doc/user/)

### Articles
- [Beginner's Guide to Neovim](https://neovim.io/doc/user/intro.html)

### Repositories
- [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim): A minimal Neovim configuration.
- [Awesome Neovim](https://github.com/rockerBOO/awesome-neovim): A curated list of Neovim plugins and resources.

---

This guide will be continually updated with more tips, workflows, and advanced techniques. Happy editing!








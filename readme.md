# This guide covers the basics all the way up to the advanced on how to use neovim
#### This is perfect for those who are just starting on vim or neovim and also for those who have some experience with neovim but want to step up their game a little more

## Introduction
### Instalation
not gonna cover that right now

## References
### YouTube links
### Neovim documentation
### Articles
### Repositories

## Getting started
### Modes
### 1. Normal mode
- It is the default mode you are in when you enter neovim. It allows you to move your cursor around and navigate trought the file.
- You can return to normal mode by pressing the **ESC** key on your keyboard.

### Command Count Motion
- **Motion** - A motion is anything that moves the cursor around
- **Count** - The count is how many times a motion is performed
    - **e.g.** - **4k** will move the cursor up 4 times
    - **e.g.** - **6j** will move the cursor down 6 times
    - **e.g.** - **5l** will move the cursor to the right 5 times
    - **e.g.** - **3h** will move the cursor to the left 4 times
- **Commad** - A command is an action to be performed on a file
- **e.g.**
    - **d4k** - will delete 4 lines above the current line
    - **d6w** - will delete the next 6 words in the current line
    - **dw** - will delete the current word (when count is not defined, it is by default 1)    

### Basic motions
- **k** - moves the cursor upwards
- **j** - moves the cursor downwards
- **l** - moves the cursor to the right
- **h** - moves the cursor to the left
- **w** - moves the cursor to the right by word
- **b** - moves the cursor to the leftt by word

### Basic commands
- **dd** - deletes the current line
- **d** - used with motion (might use a count or not) to delete text
- **y** - yak (copy) the selected text
- **c** - change the selected text (deletes and enters **Insert mode**)
- **U** - Converts selected text to uppercase
- **u** - Converts selected text to lowercase
- **>** - Indeent the selected text
- **<** - Un-indent the selected text
- **=** - Auto-indent the selected text

#

### 2. Insert mode
- You can enter insert mode by pressing **I**
- Insert mode allows you to actually edit the file you are in.
- You can identify that you are on insert mode by looking at the left bottom corner of your terminal.
### 3. Visual mode
- You can enter visual mode by pressing *V*
- Visual mode allows you to select the text you pass your cursor over. it's like highlighting the text with your cursor.
- You can identify that you are on visual mode by looking at the left bottom corner of your terminal.
### 4. Command mode
- Command mode allows you to run commands
- You can identify that you are in command mode when ther is a ":" on the bottom left corner of your terminal.

### Basic commands
- :w - it saves the file you are currently in
- :q - it exits neovim
- :wq - it saves the file you are currently in and thene exits neovim











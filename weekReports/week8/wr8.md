---
name: Misael Ramirez-Ruiz
semester: Fall 23
course: CIS 106 Linux Fundamentals
---

# Week 8 Report

## What is VIM?

* VIM is a command-line text editor that has evolved from VI. VIM stands for "Vi improved".

## What is nano?

* Nano is a quick and efficient text editor. Allows you to explore the file system system using a terminal in Linux instead of using a graphical text editor.

### Start and Quit VIM

* Starting VIM: Type the command: 'vim'
* Exiting VIM: Press esc, followed by typing ':qa!'

### Different VIM Modes:

* Insert Mode: This mode is used for writing text.
* Normal Mode: This mode is used to manipulate text.
* Command Mode: This mode is used to enter vim commands.
* Visual Mode: This mode is used to navigate and manipulate text selections.
* Select Mode: This mode is similar to visual, used to navigate and manipulate text selections.
* Ex-Mode: Similar to the command-line mode, used for batch processing.

### Insert Text in VIM

* You are able to create a file and open vim ath the same time by typing VIM followed by the file name:
  * Example: 'vim songs.txt'

* To insert text, must be in insert mode.
  * Navigate VIM by using the arrow keys.
  * Enter Key allows you to continue onto the next line.
  * Backspace allows you to delete text.

### Saving a file in VIM

* Save a text file by doing the following:
  * Must enter normal using : and W key.
    * :w - saves the file
    * :w new.txt - saves the file as new.txt
    * :wq - saves the file and exits vim
    * :wq - saves the file and closes all files open in the buffer.

### Searching for a word inside VIM

* To search for words in vim:
  * Use / and the word you are looking for to search forward.
  * Use ? and the word you are looking for to search backwards.
* The letter n will repeat the search for the next word.
* The * key will search for next occurrence of the word under the cursor.
* The # key will search backwards for the previous occurrence of the word under the cursor.

### Deleting text in VIM

* There are many ways to delete text in VIM:
  * 'dw' will delete the current word.
  * 'dd' will delete the line under the cursor.
  * 'd + /word' will delete until the given word.
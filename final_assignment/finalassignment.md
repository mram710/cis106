---
name: Misael Ramirez-Ruiz
semester: Fall 23
course: CIS 106 Linux Fundamentals
---

# Question 1

## Awk
  - Description: scripting language used for processing and displaying text.
  - Formula/Syntax: awk + options + {awk command} + file + file to save (optional)
  - 3 Examples:
    - Print the first column of every line of a file:
      - awk '{print $1}' ~/Documents/Csv/cars.csv
    - Print the last field of the /etc/passwd:
      - awk '{print $1," = ". $NF}' /etc/passwd
    - Start printing a file from a given line (exclude the first 2 lines)
      - awk 'NR > 3 { print }' /etc/passwd
  
## Cat
  - Description: used for seeing the content of a file. Also used for concatenating.
  - Formula/Syntax: cat + option + file(s) to display.
  - 3 Examples:
    - Display the content of a file with line numbers: 
      - cat -n ~/Documents/todo.md
    - Display the content of a file with line numbers excluding empty lines:
      - cat -b ~/Documents/todo.md
    - Display the content of a file suppressing repeating empty lines to a single empty line:
      - cat -s ~/Documents/todo.md
  
## Cp
  - Description: copy files and directories (use -r to copy directories)
  - Formula/Syntax: cp + files to copy + destination
  - 3 Examples:
    - To copy a file:
      - cp Downloads/wallpapers.zip Pictures/
    - To copy a directory with absolute path:
      - cp -r ~/Downloads/wallpapers ~/Pictures/
    - To copy multiple files in a single command:
      - sudo cp -r script.sh program.py home.html assets/ /var/www/html/
  
## Cut
  - Description: used to extract a specific section of each line of a file and display it to the screen.
  - Formula/Syntax: cut + option + file(s)
  - 3 Examples:
    - Display a list of all the users in your system:
      - cut -d ':' -f1 /etc/passwd
    - Display a list of all the users in your system with the user account's home directory.
      - cut -d ':' -f1,6 /etc/passwd
    - Display a list of all the users in your system with their login shell.
      - cut -d ':' -f1,7 /etc/passwd

## Grep
  - Description: used to search text in a given file. Works on a line by line basis.
  - Formula/Syntax: grep + option + search criteria + file(s)
  - 3 Examples:
    - Search for all the lines that do not contain the word 'war':
      - grep -v 'war' ~/Documents/Books/war-and-peach.txt
    - Search and display onl the matched string (pattern):
      - grep -o 'pride' ~/Documents/Books/war-and-peace.txt
    - Search for all the lines that start with a capital letter:
      - grep -n '^[A-Z]' ~/Documents/Books/war-and-peace.txt

## Head
  - Description: displays the top N number of lines of a given file.
  - Formula/Syntax: head + option + file(s)
  - 3 Examples: 
    - Display the first 10 lines of a file:
      - head ~/Documents/Book/dracula.txt
    - Display the first 5 lines of a file:
      - head -5 ~/Documents/Book/dracula.txt
    - Display the first 1 lines of a file:
      - head -1 ~/Documents/Book/dracula.txt

## Ls
  - Description: used for displaying all the files inside a given directory.
  - Formula/Syntax: ls + option + directory to list
  - 3 Examples:
    - List all the files in a given directory sorted by last modified:
      - ls -t ~/Documents
    - List all the files inside a given directory:
      - ls -lR ~/Pictures
    - List all the files in a given directory sorted by extension.
      - ls -x ~/Documents

## Man
  - Description: an interface to the system reference manuals.
  - Formula/Syntax: man + command
  - 3 Examples:
    - man + head
    - man + ls 
    - man + rm
  
## Mkdir
  - Description: used for creating a single directory or multiple directories.
  - Formula/Syntax: mkdir + the name of the directory.
  - 3 Examples:
    - Create a directory with a space in the name:
      - mkdir wallpapers/'cities usa'
    - Create multiple directories:
      - mkdir wallpapers/cars wallpapers/cities wallpapers/forest
    - Create a directory with a parent directory at the same time:
      - mkdir -p wallpapers_others/movies

## Mv
  - Description: moves and renames directories.
  - Formula/Syntax: mv + source + destination or mv + file/directory to rename + new name
  - 3 Examples:
    - To move a file from a directory to another using relative path:
      - mv Downloads/homework.pdf Documents/
    - To move a file from one directory to another combining absolute path and relative path:
      - mv Downloads/english_homework.docx /media/student/flashdrive/
    - To move multiple directories/files to a different directory:
      - mv games/ wallpapers/ rockmusic/ /media/student/flashdrive/

## Tac
  - Description: concatenate and print files in reverse.
  - Formula/Syntax: tac + option + file
  - 3 Examples:
    - Display the content of a file located in the pwd
      - tac todo.md
    - Display the content of a file using absolute path:
      - tac ~/Documents/todo.md
      - tac ~/Downloads/shopping.md

## Tail
  - Description: displays the last N number of lines of a given file.
  - Formula/Syntax: tail + option + file
  - 3 Examples:
    - Display the last 10 lines of a file:
      - tail ~/Documents/Book/dracula.txt
    - Display the last 5 lines of a file:
      - tail -5 ~/Documents/Book/dracula.txt
    - Display the last 1 line of a file:
      - tail -1 ~/Documents/Book/dracula.txt

## Touch
  - Description: used to create files or update files.
  - Formula/Syntax: touch + name of file
  - 3 Examples: 
    - touch ~/Downloads/games.txt
    - touch list_of_cars.txt script.py names.csv
    - touch "list of foods.txt"

## Tr
  - Description: used for translating or deleting characters from standard output.
  - Formula/Syntax: Standard output | tr + option + set + set
  - 3 Examples:
    - Translate one character to another (a period with a como):
      - cat file.txt | tr '.' ','
    -  Translate white space into tabs:
       - cat program.py | tr "[:space:]" '\t'
    - Translate tabs into space
      - cat file.py | tr -s "[:space:]" ' '

## Tree
  - Description: list contents of directories in a tree-like format
  - Formula/Syntax: tree + option + name of directory
  - 3 Examples:
    - tree ~/Downloads/
    - tree -p ~/Downloads/
    - tree -s ~/Downloads/

# Question 2

## How to work with multiple terminals open?
  - Using the command, screen: which is installed using 'sudo apt install screen'
    - Split vertically: ctrl + a then |
    - Split horizontally: ctrl + a then 'uppercase 'S'
    - Switch between terminals: ctrl + a then tab

## How to work manual pages?
  - man + command to see the man page you want to see. You can then navigate using the up and down key. Press Q to exit the man page.
    - Can use grep to look for certain keywords.

## How to parse (search) for specific words in the manual page?
  - After accessing the man page; you can use / followed by the word you are looking for.

## How to redirect output (> and |)
  - command output + > + file
    - Examples:
    - Save the output of a command to a file:
      - ls -lA ~ > all-files-in-home.txt 
    - Save the error generated by a command to a file:
      - ls -lA downloads/ 2> error-of-ls.txt
    - Save the error and success to the same file.
      - ls -lA downloads/ Pictures &> alloutput.txt 
  - command_1 | command_2 | command_3 | .... | command_N
    - Examples:
      - man ls | grep "human-readable"
      - head -2 file.lst | tail -1

## How to append the output of a command to a file

  - Used to overwrite any data inside the file.
    - ls -la > allmyfiles.lst
  - TO keep the old data inside the file use >>.
    - ls -la >> allmyfiles.lst

## How to use wildcards
  - For copying and moving multiple files at the same time.
    - mv *.txt ~/Downloads/ 

## How to use brace expansion
  - For creating entire directory structures in a single command
    - mkdir -p music/{jazz,rock}/{mp3files,videos,oggfiles}/new{1..3}
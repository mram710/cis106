---
name: Misael Ramirez-Ruiz
semester: Fall 23
course: CIS 106 Linux Fundamentals
---

# Week 7 Report

## Linux Commands

### Cat Command
- The cat command is used for displaying the content of a file. Cat is short for concatenate which is its command intended use.
- Formula: 'cat + option + file(s) to display'
- Example 1: 'cat todo.lst'
- Example 2: 'cat ~/Documents/todo.lst'

### Tac Command
- The tac command is used for displaying the content of a file in reverse order.
- Formula: 'tac + option + file(s) to display'
- Example 1: 'tac todo.md'   
- Example 2: 'taco ~/Documents/todo.md'

### Head Command
- The head command displays the top N number of lines of a given file. By default, it prints the first 10 lines. If more than one file name is provided then data from each file is preceded by its file name.
- Formula: 'head + option + file(s)'
- Example 1: 'head ~/Documents/Book/dracula.txt'
- Example 2: 'head -5 ~/Documents/Book/dracula.txt'

### Tail Command
- The tail command displays the last N number of lines of a given file. By default, it prints the last 10 lines. If more than one file name is provided then data from each file is preceded by its file name.
- Formula: 'tail + option + file'
- Example 1: 'tail ~/Documents/Book/dracula.txt'
- Example 2: 'tail -5 ~/Documents/Book/dracula.txt

### Cut Command
- The cut command is used to extract a specific section of each line of a file and display it to the screen.
- Formula: 'cut + option + file(s)'
- Example 1: 'cut -d ':' -f1 /etc/passwd'
- Example 2: 'cut -d ':' -f1,7 /etc/passwd'

### Paste Command
- The paste command is used for joining files horizontally in columns.
- Formula: 'paste + option + files'
- Example 1: 'paste + users.lst ip_address_lst'
- Example 2: 'paste -d ":" users1.lst ip_addresses.lst

### Sort Command
- The sort command is used for sorting files. The sort command supports sorting alphabetically, in reverse order, by number, and by month.
- The sort command follows this order unless specified otherwise:
  - Lines starting with a number will appear before lines starting with a letter.
  - Lines starting with a letter that appears earlier in the alphabet will appear before lines starting with a letter that appears later in the alphabet.
  - Lines starting with a lowercase letter will appear before lines starting the same letter in uppercase.
- Formula: 'sort + option + file'
- Example 1: 'sort users.lst'
- Example 2: 'sort -o sorted.lst users.lst'

### WC Command
- The wc command is used for printing the number of lines, characters and bytes in a file.
- Formula: 'wc + option + file(s)'
- Example 1: 'wc -m users.txt'
- Example 2: 'wc -l users.txt'

### TR Command
- The tr command is used for translating or deleting characters from standard output.
- Formula: 'Standard output | tr + option + set + set'
- Example 1: 'cat file.txt | tr '.' ',''
- Example 2: 'cat program.py | tr "[:space] '\t''

### Diff command
- The diff command compares files and displays the differences between them.
- Formula: 'diff + option + file1 + file2'
- Example 1: 'diff cars.csv cars-backup.csv'
- Example 2: 'diff -y cars.csv cars-backup.csv'
### Grep Command
- The grep command is used to search text in a given file. Grep works on a line by line basis (it matches the search criteria in a line by line basis).
- Formula: 'grep + option + search criteria + file(s)'
- Example 1: 'grep 'dracula' ~/Documents/dracula.txt' 
- Example 2: 'grep -in 'dracula' ~/Documents/Books/dracula.txt'

### Awk Command
- Awk is a scripting language used for processing and displaying text. Awk can work with a text file or from standard output. Awk performs operations line by line.
- Formula: 'awk + options + (awk command) + file + file to save (optional)
- Example 1: 'awk '{print $1}' ~/Documents/Csv/cars.csv'
- Example 2: 'awk -F: '{print $1}'  /etc/passwd'
- Example 3: 'awk -F: '{print $NF}' /etc/passwd'
- Example 4: 'awk -F: '{print $1, ' = ',$NF}' /etc/passwd'
- Example 5: 'awk 'NR > 3 {print}' /etc/passwd'

### SED Command
- SED is a stream editor that perform operations on files and standard output. For instance it can search, find and replace, insert, and deletion. By using SED you can edit files without opening them.
- Formula: 'sed options + sed script + file'
- Example 1: 'sed 's/pizza/rice/' shopping-list.lst'
- Example 2: 'sed 's/pizza/rice/4' shopping-list.lst'
- Example 3: 'sed 's/pizza/rice/g' shopping-list.lst'
- Example 4: 'sed 's/pizza/rice/3g' shopping-list.lst'
- Example 5: 'sed '3 s/pizza/rice/' shopping-list.lst'


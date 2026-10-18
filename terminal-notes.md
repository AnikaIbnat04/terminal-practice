## Terminal basics: pwd, cd, mkdir

Why it matters: The terminal runs every command in the folder I'm currently in, so I need to know where I am. If I run a command in the wrong folder, it fails or changes the wrong files.

Step 1: Typed `pwd` to see which folder I'm in (it showed my home folder).

Step 2: Typed `cd documents` to move into the Documents folder.

Step 3: Typed `mkdir terminal-practice` to create a new folder, then `cd terminal-practice` to go inside it.
Result:

```
ananna@Anannas-MacBook-Air-2 terminal-practice % pwd
/Users/ananna/documents/terminal-practice

```
Mistakes / surprises: I typed `documents` in lowercase and it still worked, but the real name is `Documents`. macOS ignores capital letters, but Linux servers don't, so I should type folder names exactly. Also, `mkdir` printed nothing, which means it worked. No message usually means success.

## Files: touch, echo, cat, > and >>

Why it matters: > replaces everything in a file with no undo, so I need to know the difference between > and >> before I touch real files. Also ,since I am learning to work on terminal i should know i to create new files and command to write and print statements there. 

Step 1: Typed `touch` to create a new file (touch hello.txt - this created a file name hello.txt)

Step 2: Typed `ls` to see what files are there in the folder

Step 3: Typed `echo "hello terminal" > hello.txt` and this wrote "hello terminal" in my hello.txt file. - The ">" replaces all previous lines. (Be careful) 
      - For example : If I type `echo "Bye terminal" > hello.txt` then "hello terminal" will be gone and new "Bye terminal" will be written in hello.txt

Step 4 : Typed `cat hello.txt` what is written. (in simple words, it prints.)

Step 5 : Typed `echo "third line" >> hello.txt` this adds to the end of the file and keeps what was already there. (which means it wont remove it's previous lines like ">" did) - This is called *Appending*


Result:

```
ananna@Anannas-MacBook-Air-2 terminal-practice % echo "hello terminal" > hello.txt
ananna@Anannas-MacBook-Air-2 terminal-practice % cat hello.txt
hello terminal
ananna@Anannas-MacBook-Air-2 terminal-practice % echo "third line" >> hello.txt
ananna@Anannas-MacBook-Air-2 terminal-practice % cat hello.txt
hello terminal
third line
ananna@Anannas-MacBook-Air-2 terminal-practice % 

```

Mistakes / surprises: I accidentally wrote '>' and '>>' as '<' and '<<' which are two different things. Also I forgot to write "> hello.txt" after "echo "Bye terminal"' 
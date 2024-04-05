# CSE15L Lab 1 Report

## cd command

> 1. no argument

**absolute path:** `/Users/gongyige/Desktop/cse15L`
![Image](cd_noArgument.jpeg)

**Explanation:** `cd` means "change directory". When given no argument, thd `cd` command take us back from the current directory `/Users/gongyige/Desktop/cse15L` to the home directory `~`, which is `/Users/gongyige`

**Error or not:** This is not an error, as `cd` takes us back to home directory as designed.

---

> 2. directory

**absolute path:** `/Users/gongyige`
![Image](cd_directory.jpeg)

**Explanation:** `cd` means "change directory". When given the directory `Desktop`, thd `cd` command take us to Desktop from the current directory `/Users/gongyige` to the directory  `/Users/gongyige/Desktop`

**Error or not:** This is not an error, as `cd` takes us to `Desktop`, one of the subdirectory of the home directory as designed.

---

> 3. file

absolute path: `/Users/gongyige/Desktop`
![Image](cd_file.jpeg)

**Explanation:** `cd` means "change directory". When given the file `demo.docx`, thd `cd` output `not a directory: demo.docx`, indicating that cd is not designed to do anything with a file.

**Error or not:** This _is_ an error, as `cd` is designed to only direct us from one _directory_ to another _directory_; when a file is given, it outputs the error: `not a directory: filename`.

---

## ls command

> 1. no argument

absolute path: `/Users/gongyige`
![Image](ls_no_argument.jpeg)

**Explanation:** `ls` means "to list all files or directory within the current working directory". When given no argument, thd `ls` lists all files or directories within the current working directory, which is the home directory here.

**Error or not:** This is not an error, as `ls` lists all the lists all files or directories within the current working directory as designed.

---

> 2. directory


absolute path: `/Users/gongyige`
![Image](ls_directory.jpeg)

**Explanation:** `ls` means "to list all files or directory within the current working directory". When given a directory, thd `ls` lists all files or directories within the _given_ directory, which is all files or directories within `Desktop`.

**Error or not:** This is not an error, as `ls` lists all the lists all files or directories within the parent directory as designed.


---

> 3. file

absolute path:`/Users/gongyige/Desktop`
![Image](ls_file.jpeg)

**Explanation:** `ls` means "to list all files or directory within the current working directory". When given a file,  `ls` just lists the file again; in this case, we give `demo.docx`, it outputs `demo.docx`.

**Error or not:** This is not an error, as `ls` lists the file itself as designed when given a file name.


---

## cat command

> 1. no argument

absolute path: `/Users/gongyige`                                      
![Image](cat_noArgument.jpeg)

**Explanation:** `cat` outputs the content of a file. When given no argument, thd `cat` command wait for a standard input and give a standard output, which means whatever command you input, it outputs the command you gave. This will stop if the user types `control+C`.

**Error or not:** This is not an error. Although it seems to be useless that the terminal just repeats what the user inputs, it is not an error.

---

> 2. directory

absolute path: `/Users/gongyige`
![Image](cat_directory.jpeg)

**Explanation:** `cat` outputs the content of a file. When given a direcotory, the `cat` command is not designed to do anything with a directory and thus outputs `cat: Desktop: Is a directory`.

**Error or not:** This _is_ an error. The `cat` command is not supposed to be given a directory as an argument, and it outputs the error message
`cat: directoryName: Is a directory` when the user does so.

---

> 3. file

absolute path:`/Users/gongyige/Desktop`
![Image](cat_file.jpeg)

**Explanation:** `cat` outputs the content of a file. When given a file, the `cat` command prints out what's within the file; in this case, what was written in the file and printed out in the terminal is "This is a demo file for lab 1, use 15L.".

**Error or not:** This is not an error. The `cat` command outputs the content of the given file as designed.


---

> AI Utilization
**prompt:**

cat with no argument in terminal

**output:** 

When you run the cat command in a terminal without providing any arguments or file names, it waits for user input from the standard input (stdin). You can type or paste text into the terminal, and cat will echo back the text you enter.

Here's an example:

# code
$ cat
Hello, world!
Hello, world!
This is a test.
This is a test.

In this case, cat is reading from the standard input. When you type a line and press Enter, cat immediately echoes back the same line. This continues until you signal the end of input by pressing Ctrl+D (on Unix-like systems) or Ctrl+Z followed by Enter (on Windows).

The cat command is often used to concatenate and display the contents of one or more files. However, when used without any arguments, it serves as a simple way to input text from the terminal and echo it back.


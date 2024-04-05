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

**Explanation:** `ls` means "to list all files or directory within the current working directory". When given no argument, thd `ls` lists all files or directories within the home directory.

**Error or not:** This is not an error, as `ls` lists all the lists all files or directories within the parent directory as designed.

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

---

## cat command

> 1. no argument

absolute path: `/Users/gongyige`                                      
![Image](cat_no_argument.jpeg)

---

> 2. directory

absolute path: `/Users/gongyige`
![Image](cat_directory.jpeg)

---

> 3. file

absolute path:`/Users/gongyige/Desktop`
![Image](cat_file.jpeg)

---


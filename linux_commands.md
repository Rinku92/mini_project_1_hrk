# Introduction to Linux and Vi

Ever wondered what text editor to use while using command line? If you faced this situation, don't worry, Vi is here to help!

First, let's start with Linux.

## History of Linux

Linus Torvalds created a project while studying computer science at University of Helsinki in 1991, which later became the Linux kernel. He wrote the program specifically for the hardware he was using and independent of an operating system because he wanted to use the functions of his new PC with an 80386 processor.

Hence the birth of Linux, which is now used by most of the Fortune 500 companies.

## Linux Commands

Now let's see some of the popular Linux commands which will help you perform the basic tasks on a Linux terminal:

**cd:**

This command is used to change directories. For example, in order to change to directory "linux2", use the following command:

`$> cd linux2`

**mkdir:**

This command is used to create new  directories. For example, in order to create a new directory "linux3", use the following command:

`$> mkdir linux3`

**cp:**

This command is used to copy files and directories from one place to another. The format is always

`$> cp <source> <destination>`

For example, in order to copy the file linux4.md into the folder linux5, use the following command:

`$> cp linux4.md linux5`

*Bonus:* This command will only create a copy of the source file or directory.

**pwd:**

This command is used to print the working directory. It is useful to know the current path or working directory and helps when lost! 

Use the following syntax:

```
$> pwd

/Users/kaustav/class601/mini_project_1_hrk 
```
**mv:**

This command is used to move a file or directory from one location to another. For example, in order to move the file linux4.md into the folder linux5, use the following command:

`$> mv linux4.md linux5`

*Bonus:* You can use this command to rename files. 

Eg.: In order to rename a file abc.txt to def.txt, use the following command:

`$> mv abc.txt def.txt`

**rm:**

This command is used to remove/delete files or directories. For example, in order to remove a file "linux3.md", use the following command:

`$> rm linux3.md`

*Bonus:* You can also remove a directory and its contents recursively using this command: 


`$> rm -r linux4`

**history:**

The history command keeps a list of all the other commands that have been run from that terminal session and then allows you to replay or reuse those commands instead of retyping them again. 
Eg:

```
$> history
  495  git push
  496  git push --set-upstream origin master
  497  cd random_repo
  498  git push
  499  git add .
  500  history

```

## Other Linux Concepts and Tricks

Let's see some of the Linux concepts and tricks commonly used in this parlance.

**Home directory:**

A home directory, also called a login directory, is the directory on Unix-like operating systems that serves as the repository for a user's personal files, directories and programs. It is also the directory that a user is first in after logging into the system.

You can go to the home directory (regardless of the current directory) using the following command:

`$> cd` 

The tilde (the wavy horizontal line character) is used to represent users' home directories on Unix-like operating systems, including users' home directories that are used to store web pages on Unix-like web servers. Thus, a user could also return to its home directory by using the tilde as an argument to cd, i.e.,

`$> cd ~ ` 

**File paths in Linux:**

 There are two types of file paths in Linux:
- Absolute filepath
- Relative filepath

*Absolute Path:*
An absolute path is defined as the specifying the location of a file or directory from the root directory(/).

For example, the file linux3.md in my working directory will be 

`$> cat /home/kaustav/linux3.md`

*Relative Path:*
Relative path is defined as the path related to the present working directly(pwd).

For example, the file linux3.md in my working directory can be read using

`$> cat linux3.md`

This can be understood by a simple image:

![File Path in Linux](images/k_absolutePathNames.jpg)

### Linux Tricks

**Using tab key for autocomplete:**

We can use the Tab key to autocomplete file and directory names while using the "*ls*" and "*cd*" commands.

For example: If I want to traverse to the path /home/kaustav/linux3.md, I can easily wite /home/kaustav/l and press the TAB key for autocomplete. 

```
$> cd /home/kaustav/l<TAB>
$> cd /home/kaustav/linux3.md
```

**Using up/down key for history:**

This is one of most useful trick I have learnt in Linux! Tired of typing similar commands over and over again? 

Then the UP/DOWN keys are here to help. Just press the UP key to traverse through the previous commands you have typed. The DOWN key is generally used to going through the history of commands.

## Using Vi

**What is Vi?**

The Vi editor is the most popular and classic text editor in the Linux family. It is included with most Linux systems, even embedded ones. Below are some of the reasons why it is popular:

- It is available in almost all Linux Distributions
- It works the same across different platforms and Distributions
- It is user-friendly. Hence, millions of Linux users love it and use it for their editing needs

**Command Mode**

This is what you’ll see when you open a file in vi. It looks like you can just start typing, but you can’t. Vi is a modal text editor, and it opens in command mode. 

In this mode, you can, move the cursor and cut, copy, paste the text. Position the cursor at the left or right side of the text you want to copy and press the v key. Move your cursor to select text, and then press y to copy the selected text or x to cut it. Position your cursor at the desired location and press the p key to paste the text you copied or cut.

**References:**
1. https://en.wikipedia.org/wiki/History_of_Linux
2. http://www.linfo.org/home_directory.html
3. https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/

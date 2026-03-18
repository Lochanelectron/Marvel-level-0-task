# Command Line Basics Report

## Introduction

In this task, I learned some basic command line operations in Linux. I used the Kali Linux terminal, which works almost the same as Ubuntu. The goal was to practice creating folders, files, and using simple terminal commands.

## Creating a Folder

First, I created a folder named `test`.

```bash
mkdir test
```

Then I moved into that folder.

```bash
cd test
```

## Creating a Blank File

Inside the folder, I created an empty file without using a text editor.

```bash
touch file1.txt
```

## Listing Files

To see the files inside the folder, I used the `ls` command.

```bash
ls
```

## Creating Multiple Folders

Next, I created many folders automatically using a loop. The folders were named using letters and numbers such as `A1`, `B56`, etc.

```bash
for letter in {A..Z}; do
  for number in {1..100}; do
    mkdir ${letter}${number}
  done
done
```

This created **2600 folders** in total.

## Concatenating Two Files

I created two text files with some random text.

```bash
echo "Hello this is file one" > fileA.txt
echo "And this is file two" > fileB.txt
```

Then I combined and displayed both files using the `cat` command.

```bash
cat fileA.txt fileB.txt
```

## Conclusion

In this task, I practiced basic Linux terminal commands like creating folders, creating files, listing files, and combining text files. This helped me understand how to use the command line in a simple way.


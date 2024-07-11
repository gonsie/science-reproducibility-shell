<!--
  <<< Author notes: Step 2 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-2-notes.
-->

# Week 2: More Shell commands
In the second week:
- we will learn more about the Shell
- we will use Shell commands that could be used to check the content of the files
- we will use `pipes` in Shell commands

## 1 :book: More about Shell
Software Carpentry provide an excellent introduction to Shell, I recommend reading these two parts to learn about Shell and command syntax:
- [Introduction to Shell](https://swcarpentry.github.io/shell-novice/01-intro.html) will give you more overview
- [General syntax of the Shell command](https://swcarpentry.github.io/shell-novice/02-filedir.html#general-syntax-of-a-shell-command)

## 2 :book: Week 1 review
If you would like to read more from Software Carpentry to review week 1:
- [Navigating Files and Directories](https://swcarpentry.github.io/shell-novice/02-filedir.html) 
- [Working With Files and Directories](https://swcarpentry.github.io/shell-novice/03-create.html)

## 3. :eyes: Working with files content
- :eyes: **Video** :eyes:: Continue watching the [ABCD/ReproNim video](https://youtu.be/SyKmry47SsY?si=EzGkBtHpRRkFqtNH&t=1203) (the video should open at timestamp 20m3s, and you should watch till 28m45s)
- Use `man` to read more about commands:

## 4. :keyboard: Practice using new commands 

In the new branch that was created for this week `week2` you will find a new directory `week2` that will be used as a working directory for this week. Practice using new commands (especially `cat`, `head` and `tail`) for the files in `ex1` and `ex2` directories.
Use `man` to learn about different options.

  
> [!TIP]
> If you don't remember how to open Codespace, create a new file and add to the repository, you can review instruction from the previous week [here](./week1/Readme.md)


## 5. :keyboard: :white_check_mark: Exercise 1: Merging content of the files

In the new branch that was created for this week `week2` you will find a new directory `week2` that will be used as a working directory for this week. You should specifically use `week2/ex1` for the first exercise. The directory already have 3 files.

Your first exercise will be to open Codespace and merge content of the files in the alphabetic order to a new file `week2/ex1/output.txt`.


## 6. :keyboard: :white_check_mark: Exercise 2: Using Pipes to work with file content

In the `week2/ex2` directory you have a file with Massachusetts cities ordered by the population size. I want you to use pipes to sort the cities alphabetically and create a new file `week2/ex2/output.txt` with the top 10 cities.  

##

> [!IMPORTANT]
> Update the repository in  order to move to the next week/part of the course:
>  - Create a Pull Request to the `main` branch
>  - Check the status of tests
>  - If all tests pass, merge the Pull Request, this should update a new `README.md` on the main page of the repository (you can reload the page after 30-60s if you don't see the new content)

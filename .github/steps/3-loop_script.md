<!--
  <<< Author notes: Step 3 >>>
  Start this step by acknowledging the previous step.
  Define terms and link to docs.github.com.
  TBD-step-3-notes.
-->

# Week 3

The goal of this week is:
- automate task using loops
- automate tasks using Shell scripts
- use Shell variables

## 1. :book: Week 2 review
If you would like to read more from Software Carpentry to review week 2:
- [Pipes and Filters](https://swcarpentry.github.io/shell-novice/04-pipefilter.html)


## 2. :book: :eyes: For loops and simple scripts

#### Loops in bash 
I told you at the beginning that Shell is good in task automation. One of the way to automate a task is to use for loop. This is a syntax of the bash loop for a simple task of writing 3 names:
```
for i in John David Adam;
do echo $i is my friend;
done
```
Note that you can enter one line at a time to your terminal, bash will know to wait for your instruction after you enter `for i in John David Adam;` and will not do anything before you get to `done`.

You could also enter everything in one line:
```
for i in John David Adam; do echo $i is my friend; done
```

#### Scripts
Another way of automatic your work is to move your commands to a script, this is especially important if you have multiple tasks to do. For the example above, you can create a script, e.g., `touch script_name.sh` and include this in the content:
```
for i in John David Adam;
do echo $i is my friend;
done
```
In order to run the script in the terminal, you can run `bash script_name.sh` (sometimes might be needed `/bin/bash script_name.sh`).

#### Scripts with arguments
In the same way we could use argument with bash commands, e.g., `cat file.txt`, we could provide argument to our bash script. We could create a script that uses the first argument:
```
echo "$1" is my friend
```
Now you can run the script: `bash script_name.sh Adam`.

If we want to combine it with the loop and you don't know how many arguments you want to provide, you can use `"$@"`:
```
for i in "$@";
do echo $i is my friend;
done
```
and run the code with `bash script_name.sh John David Adam`.

#### Shebang
You sometimes can see an additional line in bash scripts `#!/bin/bash`.
It is called "shebang" and it would be the first line in the script. 
The general rule is that shebang starts with #! and is followed by the command interpreting the script (`/bin/bash` in our example`).
When you have shebang, running `./script_name.sh` is analogous to calling `/bin/bash ./script_name.sh`.


### :eyes: **Video** :eyes:
Continue watching the [ABCD/ReproNim video](https://youtu.be/SyKmry47SsY?si=LBNjhN1olIAgDoEk&t=1734) (the video should open at timestamp 28m54, and you should watch till 33m)

## 3. :keyboard: :white_check_mark: Exercise 1: Using a loop

In the new branch that was created for this week `week3` you will find a new directory `week3` that will be used as a working directory for this week. You should specifically use `week2/ex1` for the first exercise. The directory already have some files that will be used for the exercise.

Last week, we merged 3 files into one using `cat` command. This time, you have 10 files, and the idea is to use a loop to merge them together. Write the output to  `week3/output_loop.txt`.

> [!TIP]
> If you don't remember how to open Codespace, create a new file and add to the repository, you can review instruction from the previous week [here](./week1/Readme.md)

## 4. :keyboard: :white_check_mark: Exercise 1: Create a script

Do the same as in part 3, but this time create a script `week3/script.sh` to create `week3/output_script.txt`.

In addition, the script should write the names of all the files together with the number of lines in each file to `week3/output_stats.txt`

## 5. :keyboard: :white_check_mark: Exercise 2: Create a script with an input

Update the `script.sh` from the previous point to use the name of the outputs provided as command line arguments, e.g. `./script_input.sh output_script_1.txt output_stats_1.txt`. 

##

> [!IMPORTANT]
> Update the repository in  order to move to the next week/part of the course:
>  - Create a Pull Request to the `main` branch
>  - Check the status of tests
>  - If all tests pass, merge the Pull Request, this should update a new `README.md` on the main page of the repository (you can reload the page after 30-60s if you don't see the new content)

<!--
  <<< Author notes: Step 1 >>>
  Choose 3-5 steps for your course.
  The first step is always the hardest, so pick something easy!
  Link to docs.github.com for further explanations.
  Encourage users to open new tabs for steps!
  TBD-step-1-notes.
-->

# Week 1: Shell overview and using shell in codespace

In the first part of the course, we will learn basic information about the Shell and popular Shell commands.
We will practice using the command in the GitHub codespace.

## 1 :book: :eyes: What is Shell

A Unix shell is a command-line interpreter or shell that provides a command line user interface for Unix-like operating systems. The shell is both an interactive command language and a scripting language, and is used by the operating system to control the execution of the system using shell scripts.

Shell commonly refers to the UNIX shell environment, provides a command line user interface for Unix-like operating systems.
Because desired actions are expressed as typed commands, it is possible to script (program) sets of those commands to be (re-)executed repetitively or conditionally. 
For example, it provides constructs for loops, functions, and conditions. 
In contrast to GUIs (graphical user interfaces), it allows for  automation via scripting.

- :eyes: **Video** :eyes: Watch the first 20min video of my presentation from [ABCD/RerproNim course](https://www.abcd-repronim.org/week2.html) for [introduction to shell and a short demo session](https://www.youtube.com/watch?v=SyKmry47SsY) (I will share more of the video later during this course, so no need to watch more than till 19m54s)


> Questions:
> - Do you know what is the main difference between working with GUI and working with Shell?
> - Do you know how can you determine what shell you’re currently in?
> - Do you know what is bash?




## 2 :book: :keyboard: Working with GitHub and Codespace

As I mentioned before we will be using GitHub and GitHub Skills templates, if you are not familiar with GitHub and exercise, and you haven't had a chance to complete these 2 short GitHub courses, this is the time to do it before you start using the knowledge for this course.

- [Introduction to GitHub](https://github.com/skills/introduction-to-github)
- [Code with Codespace](https://github.com/skills/code-with-codespaces) (the first 3 steps are enough for this course)

> Questions:
> - Do you know what are the branches in this repository? Do you know how to change the branch?
> - Do you know how to create a Pull Request (i.e., update the main branch)?
> - Do you know how to open Codepsace?

## 3 :eyes: :keyboard: Exercise 1: Practicing using shell commands

> [!TIP]
> - I recommend opening another browser tab with this repository, so you can keep these instructions open for reference all the time.
> - This is our first exercise (I will use :keyboard: for all exercises), so I will provide very detailed steps to guide you.
Each execrice will have a similar structure, so it should become automatic very soon.
> - :eyes: **Demo** :eyes: You can follow this demo TODO if you have any problems

1. Opening Codespace with terminal
  -  Start from the landing page of your repository opened in new tab.
  - Change the branch to "part1" (you should see a new content that was not in the `main` branch)
  - Click the green "Code" button located in the middle of the page.
  - Select the Codespaces tab in the box that pops up and then click the "Create codespace on part1" button.
  - Verify your codespace is running. The browser should contain a VS Code web-based editor and a terminal.
2. Practice using the command you learn about from the video in the first section. Here is a list and some examples:
  -  `echo $SHELL`
  -  `ls`, `ls -l`
  -  try using `man` to learn more about the commands, e.g. `man ls`
  -  `mkdir tmp` (we will not be saving content in this directory)
  -  `cd tmp` (move to this directory for practicing more commands)
  -  `pwd` (it should be the name of the repository)
  -  `touch <filename>` (if something is in brackets <> that means you should replace it with your own name, e.g. `touch new_file.txt`, note it is better to not use spaces in the filename)
  -  `mv <existing_file> <new_file>` 
  -  `cp <existing_file> <new_file>` (you can practice using wildcart `*`)
  -  practice using bash history (:arrow_up:, `ctrl` + `r`, `history`)
  -  practice using `tab` completion
3. Remove the `tmp` directory to keep clean repository
  - `cd ..` (move one directory higher in the hierarchy)
  - `pwd` (it should be the same as previously, the name of the repository)
  - `rm -r tmp` (remove the `tmp` directory)
    
## 4 :eyes: :keyboard: :white_check_mark: Exercise 2: Creating new file

> [!TIP]
> - This exercise has :keyboard: and :white_check_mark:, that means you will have a specific task and the output will be checked by automatic tests I wrote for this course, and the repository will move to **Part 2** after the task is completed.
> - This is our first exercise of this type, so I will provide very detailed steps to guide you.
> - :eyes: **Demo** :eyes: You can follow this demo TODO if you have any problems

1. Go to terminal in Codespace (you can use the one that you opened in part 3, or follow the instruction from part 3 to open again)
2. Create a new file (`week1/file1.txt`) to the repository with content "Hello!":
  - Go to `week1` directory (if you don't see this directory, you're likely in wrong branch)
  - Create a new file `file1.txt` with a content "Hello" (you can use `touch` or/and `echo` command)
  - Add a new file to the repository and commit the changes
3. Update the changes to the `main` branch of the repository
  - Create a Pull Request to the `main` branch
  - Check the status of tests
  - If all tests pass, merge the Pull Request, this should update a new `README.md` on the main page of the repository (you can reload the page after 30-60s if you don't see the new content)

> [!IMPORTANT]
> Following all the steps from part 4, including creating and merging the Pull Request, is necessary to move to the next parts of the course.

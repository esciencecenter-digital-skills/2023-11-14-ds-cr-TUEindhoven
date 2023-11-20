![](https://i.imgur.com/iywjz8s.png)


# Day 1 - Collaborative Document

2023-11-14 Good practices in Research Software (2023-11-14-ds-cr-TUEindhoven)

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: [https://tinyurl.com/2023-11-14-hack](https://tinyurl.com/2023-11-14-hack)

Collaborative Document day 1: [https://tinyurl.com/2023-11-14-hack](https://tinyurl.com/2023-11-14-hack)

Collaborative Document day 2: [https://tinyurl.com/2023-11-15-hack](https://tinyurl.com/2023-11-15-hack)


##  🫱🏽‍🫲🏻 Code of Conduct

Participants are expected to follow these guidelines:
* Use welcoming and inclusive language.
* Be respectful of different viewpoints and experiences.
* Gracefully accept constructive criticism.
* Focus on what is best for the community.
* Show courtesy and respect towards other community members.
 
 For more details, see [here](https://docs.carpentries.org/topic_folders/policies/code-of-conduct.html).

Want to report a Code of Conduct incident and you prefer to do it anonymously? You can do it [here](https://goo.gl/forms/KoUfO53Za3apOuOK2).

## ⚖️ License

All content is publicly available under the Creative Commons Attribution License: [creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/).

## 🙋Getting help

To ask a question, just raise your hand.

If you need help from a helper, place a post-it that says HELP on your laptop lid. A helper will come to assist you as soon as possible. We use the post-it with OK to signal when you're done with something.

## 🖥 Workshop website

[https://esciencecenter-digital-skills.github.io/2023-11-14-ds-cr-TUEindhoven/](https://esciencecenter-digital-skills.github.io/2023-11-14-ds-cr-TUEindhoven/)

🛠 Setup

We will assume everyone can access the command line on their laptop and managed to follow these [**setup instructions**](https://esciencecenter-digital-skills.github.io/2023-11-14-ds-cr-TUEindhoven/#:~:text=the%20CET%20timezone.-,Setup,-To%20participate%20in).

Please put a pink post-it note on you laptop lid, if you need a bit more help with the setup.

## 👩‍🏫👩‍💻🎓 Instructors

Olga Lyashevska, Sven van der Burg, Carsten Schnober

## 🧑‍🙋 Helpers

Carsten Schnober

## 👩‍💻👩‍💼👨‍🔬🧑‍🔬🧑‍🚀🧙‍♂️🔧 Roll Call
Name/ pronouns (optional) / job, role / social media (twitter, github, ...) / background or interests (optional) / city

## 🗓️ Agenda

|  Time | Topic                             |
| -----:|:--------------------------------- |
| 09:30 | Welcome and icebreaker            |
| 09:45 | Workshop Introduction             |
| 10:00 | Version control with Git          |
| 10:30 | **Coffee break**                  |
| 10:45 | Version control with Git          |
| 11:30 | **Coffee break**                  |
| 11:45 | Version control with Git          |
| 12:30 | **Lunch Break**                   |
| 13:30 | Collaboration with Git and GitHub |
| 14:15 | **Coffee break**                  |
| 14:30 | Collaboration with Git and GitHub |
| 15:15 | **Coffee break**                  | 
| 15:30 | Collaboration with Git and GitHub |
| 16:15 | Wrap-up                           |
| 16:30 | END                               |
	

## 🏢 Location logistics
* Coffee and toilets
* Emergency exit
* Wifi

## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl .

## 🔧 Exercises


### Exploring history exercise

#### 1. Recovering Older Versions of a File
Jennifer has made changes to the Python script that she has been working on for weeks, and the modifications she made this morning “broke” the script and it no longer runs. She has spent ~ 1hr trying to fix it, with no luck…

Luckily, she has been keeping track of her project’s versions using Git! Which commands below will let her recover the last committed version of her Python script called `data_cruncher.py?` Multiple options might be correct:

1. `$ git checkout HEAD`
2. `$ git checkout HEAD data_cruncher.py`
3. `$ git checkout HEAD~1 data_cruncher.py`
4. `$ git checkout <unique ID of last commit> data_cruncher.py`
 
   

#### 2. (optional) Understanding Workflow and History

What is the output of the last command in
```
$ cd planets
$ echo "Venus is beautiful and full of love" > venus.txt
$ git add venus.txt
$ echo "Venus is too hot to be suitable as a base" >> venus.txt
$ git commit -m "Comment on Venus as an unsuitable base"
$ git checkout HEAD venus.txt
$ cat venus.txt #this will print the contents of venus.txt to the screen
```
1. Venus is too hot to be suitable as a base
2. Venus is beautiful and full of love
3. Venus is beautiful and full of love
   Venus is too hot to be suitable as a base
4. Error because you have changed venus.txt without committing the changes

5. venus is beautiful and full of love. Venus is too hot to be suitable for a base 


#### 3. (optional) Reverting a Commit

Jennifer is collaborating on her Python script with her colleagues and realizes her last commit to the project’s repository contained an error and she wants to undo it. `git revert [erroneous commit ID]` will create a new commit that reverses Jennifer’s erroneous commit. Therefore `git revert` is different to `git checkout [commit ID]` because `git checkout` returns the files within the local repository to a previous state, whereas `git revert` reverses changes committed to the local and project repositories.
Below are the right steps and explanations for Jennifer to use `git revert`, what is the missing command?

1. `________ # Look at the git history of the project to find the commit ID`
2. `Copy the ID (the first few characters of the ID, e.g. 0b1d055).`
3. `git revert [commit ID]`
4. Type in the new commit message.
5. Save and close

> The command `git log` lists project history with commit IDs.

> The command `git show HEAD` shows changes made at the latest commit, and lists the commit ID; however, Jennifer should double-check it is the correct commit, and no one else has committed changes to the repository.
 
### Optional exercises during SSH setup check
#### 1. CHECKING UNDERSTANDING OF `git diff`
Consider this command: `git diff HEAD~9 mars.txt`. What do you predict this command will do if you execute it? What happens when you do execute it? Why?


Try another command, `git diff [ID] mars.txt`, where [ID] is replaced with the unique identifier for your most recent commit. What do you think will happen, and what does happen?

#### 2. GETTING RID OF STAGED CHANGES
`git checkout` can be used to restore a previous commit when unstaged changes have been made, but will it also work for changes that have been staged but not committed? Make a change to mars.txt, add that change using `git add`, then use `git checkout` to see if you can remove your change.

#### 3. IGNORING NESTED FILES
Given a directory structure that looks like:

```bash
results/data
results/plots
```

How would you ignore only `results/plots` and not `results/data`?


#### 4. INCLUDING SPECIFIC FILES
How would you ignore all `.csv` files in your root directory except for final.csv? Hint: Find out what `!` (the exclamation point operator) does


### 'The remote' exercises
#### GitHub GUI

Browse to your `planets` repository on GitHub. Under the Code tab, find and click on the text that says “XX commits” (where “XX” is some number). Hover over, and click on, the three buttons to the right of each commit. What information can you gather/explore from these buttons? How would you get that same information in the shell?

#### (optional) Push vs. Commit

In this lesson, we introduced the `“git push”` command. How is `“git push”` different from `“git commit”`?


#### (optional) GITHUB TIMESTAMP
Create a remote repository on GitHub. Push the contents of your local repository to the remote. Make changes to your local repository and push these changes. Go to the repo you just created on GitHub and check the [timestamps](https://swcarpentry.github.io/git-novice/reference.html#timestamp) of the files. How does GitHub record times, and why?


### Exercise: Working as a project collaborator (in pairs)

Do this exercise in pairs.

#### Part 1
- PERSON A: Create an issue in the repository
- PERSON B: Clone this repository to your system
- PERSON B: Create a new branch
- PERSON B: Make the changes requested in the issue
- PERSON B: Push the changes to the remote repository on GitHub
- PERSON B: submit a Pull Request, refer to the issue (e.g. "Closes #1")

#### Part 2
- PERSON A: review the Pull Request
- PERSON B: address the comments
- PERSON A: approve the Pull Request
- PERSON B: merge the Pull Request

### Exercise: (optional) Working as an external contributor (in pairs)

#### Part 1
- PERSON A: Create an issue in Person B's repository
- PERSON A: Fork the repository to their own (= Person A's) account
- PERSON A: Clone the repository, make changes, push them back to the fork
- PERSON A: Submit a Pull Request from the fork to the original repository

#### Part 2
- PERSON B: Make a change in the original repository in the same place as person A's proposed changes
- PERSON A: Solve the merge conflict in the Pull Request
- PERSON B: Review/Approve the Pull Request
- PERSON B: merge the Pull Request




## 🧠 Collaborative Notes

### Git and GitHub

#### Quiz 1/2: Which commit message should I choose?

Make it short, descriptive and imperative!
-> Answer 3 "Discuss origin of the project"

#### Quiz 2/2: Which command saves `myfiles.txt` to my Git Repo?

Answer 3 is correct:

```shell!
$ git add myfile.txt
$ git commit -m "my recent changes"
```

#### Git Commands

##### Configuration

Is Git installed properly?
```shell!
$ git --version
git version 2.34.1
```

Configure Git:
```shell!
$ git config --global user.name
Your Name

$ git config --global user.name "My Name"

$ git config --global user.email
your.name@email.com

$ git config --global user.email "my.new@email.org"
```

Configure editor:
```shell!
$ git config --global core.editor
vim

$ git config --global core.editor "nano"
OR
$ git config --global core.editor "nano -w"
```

Configure default branch:
```shell!
$ git config --global init.defaultBranch

$ git config --global init.defaultBranch "main"
```

List configuration:
```shell!
$ git config --list
user.name=...
user.email=...
...
```

Edit configuration file:
```shell!
git config --global --edit
```
Press Ctrl+X to exit


Get help:
```shell!
$ git --help
...
$ git config --help
...
```

##### Set up a Git Repository

```shell!
$ cd ~/Desktop/
$ mkdir planets
$ cd planets/
$ git init
Initialized empty Git repository in .../Desktop/planets/.git/
$ ls -al
total 0
drwxr-xr-x@ 3 username  group   96 Nov 14 11:29 .
drwx------+ 5 username  group  160 Nov 14 11:29 ..
drwxr-xr-x  9 username  group  288 Nov 14 11:29 .git
$ git status
On branch main

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

Create a new file:
```shell!
$ nano mars.txt
```
Add some content to the new file `mars.txt`.

```shell!
$ cat mars.txt
Cold and dry.
```

```shell!
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	mars.txt

nothing added to commit but untracked files present (use "git add" to track)
```
Add new file to repository (stage):
```shell!
$ git add mars.txt
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   mars.txt
```
Commit new file to repository:
```shell!
$ git commit -m "Start notes on Mars"
[main (root-commit) 4109e5d] Start notes on Mars
 1 file changed, 2 insertions(+)
 create mode 100644 mars.txt
```

See what was committed:
```shell!
$ git log
commit 4109e5d9b864c1b87d786b77f874dbb8e6300f44 (HEAD -> main)
Author: Carsten Schnober <c.schnober@esciencecenter.nl>
Date:   Tue Nov 14 11:39:09 2023 +0100

    Start notes on Mars

```
Change your file:
```shell!
$ nano mars.txt
```
Check status
```shell!
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   mars.txt

no changes added to commit (use "git add" and/or "git commit -a")

```
See changes:
```shell!
$ git diff
diff --git a/mars.txt b/mars.txt
index c276d6a..e4a38f9 100644
--- a/mars.txt
+++ b/mars.txt
@@ -1,2 +1,2 @@
 Cold and dry.
-
+The two moons may be a problem.

```
Repeat the `git add` command from above.

See changes that have been staged:
```shell!
$ git diff --staged
diff --git a/mars.txt b/mars.txt
index c276d6a..e4a38f9 100644
--- a/mars.txt
+++ b/mars.txt
@@ -1,2 +1,2 @@
 Cold and dry.
-
+The two moons may be a problem.
```
Commit the staged change with `git commit` like above. 


See changes since previous commit(s), e.g. `HEAD~1`:
```shell!
$ git diff HEAD~1 mars.txt
diff --git a/mars.txt b/mars.txt
index c276d6a..e4a38f9 100644
--- a/mars.txt
+++ b/mars.txt
@@ -1,2 +1,2 @@
 Cold and dry.
-
+The two moons may be a problem.
```

Compare specific commit; every commit id is different, copy it from the `git log` output:

```shell!
$ git log
commit 8a1c0b0444e06ff0d7133f3eae98792721451d8c (HEAD -> main)
Author: Carsten Schnober <c.schnober@esciencecenter.nl>
Date:   Tue Nov 14 13:41:04 2023 +0100

    Add line.

commit 4109e5d9b864c1b87d786b77f874dbb8e6300f44
Author: Carsten Schnober <c.schnober@esciencecenter.nl>
Date:   Tue Nov 14 11:39:09 2023 +0100

    Start notes on Mars

$ git diff 8a1c0b04 HEAD~1
diff --git a/mars.txt b/mars.txt
index e4a38f9..c276d6a 100644
--- a/mars.txt
+++ b/mars.txt
@@ -1,2 +1,2 @@
 Cold and dry.
-The two moons may be a problem.

```

Show a specific commit for a file:
```shell!
$ git show 8a1c0b04 mars.txt
commit 8a1c0b0444e06ff0d7133f3eae98792721451d8c (HEAD -> main)
Author: Carsten Schnober <c.schnober@esciencecenter.nl>
Date:   Tue Nov 14 13:41:04 2023 +0100

    Add line.

diff --git a/mars.txt b/mars.txt
index c276d6a..e4a38f9 100644
--- a/mars.txt
+++ b/mars.txt
@@ -1,2 +1,2 @@
 Cold and dry.
-
```

Go back to specific commit (and to `HEAD`):
```shell!
$ git checkout 4109e5d9 mars.txt
Updated 1 path from 52f309b
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   mars.txt
$ git checkout HEAD mars.txt
Updated 1 path from 90f00c2
$ git status
On branch main
nothing to commit, working tree clean        
```

Mark files for ignoring by adding them to `.gitignore:
```shell!
nano .gitignore
```
For instance, add `*.csv` to ignore all files ending with `.csv`.

Check which files are being ignored:
```shell!
$ git check-ignore
```

Add remote (GitHub) repository (name: `origin`) and push local changes:
```shell!
$ git remote add origin git@github.com:carschno/planets.git
$ git branch -M main
$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 10 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 505 bytes | 505.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:carschno/planets.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```
Get changes (if any) from remote (`origin`):
```shell!
% git pull origin main 
From github.com:carschno/planets
 * branch            main       -> FETCH_HEAD
Already up to date.
```
 


## 💬Feedback for the morning
Please give us some feedback about this morning, let us know one (or more) thing that went well and one thing that can be improved. This can be anything: the pace, the content, the relevance to your work, the interactiveness, how we answer questions. We use your feedback to tune the rest of the workshop to your needs! 

### What went well?

- Good refresher for people with some experience with Git
- Good explaination.
- Good balance between theory and practical use.
- Very usefull to do it in parallel with the instructor and follow on the screen.
- I like the pace of the training, but it could be better to speed-up in simple topics
- The tutorial is put forward in simple language
- Very good explanation and clarity of topics
- Keep the breaks because it is extremely important. Three breaks should be enough.

### What can be improved?
- Explain what we are doing in prospect of how changes are being tracked. How commits are being used. Give examples.
- Possibly one break in the morning is sufficient. 
- You could speed-up for more advanced topics
- agree: You could speed-up for more advanced topics
- Provide an onlin pre training for those who are not familiar with some topics.
-
-

## 💬Feedback for afternoon
Please give us some feedback about this afternoon, let us know one (or more) thing that went well and one thing that can be improved. This can be anything: the pace, the content, the relevance to your work, the interactiveness, how we answer questions. We use your feedback to tune the rest of the workshop to your needs! 

### What went well?
- Good demonstration for the collaboration work
- Agree with: Good demonstration for the collaboration work
- 
-
-
-
-
-

### What can be improved?
- Some questions are not explained in time such as git revert
- The revert part and exercise for Collaboration didn't worked for me in a short time frame. 
-
-
-

### Tomorrow:
- Other location: Wednesday, November 15: TU/e campus, Zwarte Doos 1.03 (
https://maps.app.goo.gl/FSX7LmHswKWEMqCs7
). You enter from the restaurant, the room is directly upstairs across the staircase.
- start 9:30 sharp (you can come earlier for questions and chit-chat)
- Bring your post-its and name tag
## 📚 Resources

### eScience Center:
- Subscribe to our [newsletter](http://eepurl.com/dtjzwP)
- [Website](https://www.esciencecenter.nl/)
- [Upcoming workshops](https://www.esciencecenter.nl/events/?f-workshops/)

### Other resources
- [Documentation for git-diff](https://git-scm.com/docs/git-diff), including details about the output format
- Post about [atomic commits](https://www.pauline-vos.nl/atomic-commits/)
- [The Utopic git history](https://blog.esciencecenter.nl/the-utopic-git-history-d44b81c09593)
- Example [Matlab `.gitignore` file](https://github.com/github/gitignore/blob/main/Global/MATLAB.gitignore)
- Example [Python `.gitignore` file](https://github.com/fair-workflows/nanopub/blob/main/.gitignore)

### Slides:
[Slides](https://lyashevska.github.io/ds-cr-slides/)
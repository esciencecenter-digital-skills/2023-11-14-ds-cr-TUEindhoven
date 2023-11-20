![](https://i.imgur.com/iywjz8s.png)


# Day 2 - Collaborative Document

2023-11-14 Good practices in Research Software (2023-11-14-ds-cr-TUEindhoven)

Welcome to The Workshop Collaborative Document.

This Document is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

----------------------------------------------------------------------------

This is the Document for today: [https://tinyurl.com/2023-11-15-hack](https://tinyurl.com/2023-11-15-hack)

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

If you need help from a helper, place a pink post-it note on your laptop lid. A helper will come to assist you as soon as possible.

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


|  Time | Topic                                  |
| -----:|:-------------------------------------- |
| 09:30 | Welcome and icebreaker                 |
| 09:45 | Writing modular code                   |
| 10:30 | **Coffee break**                       |
| 10:40 | Writing modular code                   |
| 11:30 | **Coffee break**                       |
| 11:40 | Documentation                          |
| 12:30 | **Lunch Break**                        |
| 13:30 | Introduction to testing                |
| 14:20 | **Coffee break**                       |
| 14:30 | Introduction to Continuous Integration |
| 15:20 | **Coffee break**                       |
| 15:30 | Introduction to packaging
|
| 16:15 | Wrap-up                                |
| 16:30 | END                                    |
|       |                                        |

## 🏢 Location logistics
* Coffee and toilets
* Emergency exit
* Wifi

## 🎓 Certificate of attendance
If you attend the full workshop you can request a certificate of attendance by emailing to training@esciencecenter.nl .

## 🔧 Exercises
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


### Exercise: Modularity

Look at the following code.

Extract functions from it without changing its functionality.

https://raw.githubusercontent.com/lyashevska/modular-code-dev/main/conversion.py

Example answer: 
https://raw.githubusercontent.com/lyashevska/modular-code-dev/main/conversion_mod.py



What functions did you create?
What strategies did you use to identify them?

Share your answers in the collaborative document

### Documentation


#### Exercise: Think of good and bad examples 
Write down your thoughts in the collaborative documents.
Respond with emojis :+1: :scream_cat: to your colleagues' answers.
- Think of projects of which you like the documentation. What do you like about them?
- Think of projects for which you don’t like the documentation. What don’t you like about them? Are you missing anything?

**NB: You can choose a mature library with lots of users for this exercise, but try to also think of less mature projects you had to collaborate on, or papers you had to reproduce.**

---

 #### Exercise README: Draft or improve a README for one of your recent projects

Try to draft a brief README or review a README which you have written for one of your projects.

You can work individually, but you could also discuss whether anything can be improved on your neighbour's README file(s).

Think about the user (which can be a future you) of your project, what does this user need to know to use or contribute to the project? And how do you make your project attractive to use or contribute to?

A good README should include:
- A descriptive project title
- Motivation (why the project exists)
- How to setup
- Copy-pastable quick start code example
- Recommended citation

(Optional): Try the https://hemingwayapp.com/ to analyse your README file and make your writing bold and clear.


 ---
 ### Exercise: Test-driven development

The function `fizz_buzz()` takes an integer argument and returns it, BUT:

- It fails on zero or negative numbers
- It returns "Fizz" on multiples of 3
- It returns "Buzz" on multiples of 5
- It instead returns "FizzBuzz" on multiples of 3 and 5

You will use test-driven development to write this function.

1. Create an empty function `fizz_buzz()`
2. Go through the conditions listed above, one by one:
    1. Write a test for the condition
    2. Edit the `fizz_buzz()` function until the test passes
3. Share your tests in the collaborative document.

What did you think of this style of developing?

### Official solution fizz buzz
```python
import pytest

def fizz_buzz(input):
    if input <= 0:
        raise ValueError('Negative or zero input not allowed')
    if input % 3 == 0 and input % 5 == 0:
        return 'FizzBuzz'
    if input % 3 == 0:
        return 'Fizz'
    if input % 5 == 0:
        return 'Buzz'
    return input

def test_fizz_buzz():
    with pytest.raises(ValueError):
        fizz_buzz(0)
    with pytest.raises(ValueError):
        fizz_buzz(-2)
    assert fizz_buzz(1) == 1
    assert fizz_buzz(3) == 'Fizz'
    assert fizz_buzz(4) == 4
    assert fizz_buzz(5) == 'Buzz'
    assert fizz_buzz(6) == 'Fizz'
    assert fizz_buzz(10) == 'Buzz'
    assert fizz_buzz(15) == 'FizzBuzz'

```

### Exercise: Full-cycle collaborative workflow

The exercise takes 30-40 minutes.

In this exercise, everybody will:

A. Set up automated tests with GitHub Actions
B. Make test fail / find a bug in their repository
C. Open an issue in their repository
D. Then each one will clone the repo of one of their exercise partners, fix the bug, and open a pull request (GitHub)
E. Everybody then merges their co-worker’s change


#### Step 1: Create a new repository on GitHub

- Select a different repository name than your colleagues (otherwise forking the same name will be strange)
- Before you create the repository, select “Initialize this repository with a README” (otherwise you try to clone an empty repo).
- Share the repository URL with your exercise group via shared document or chat

#### Step 2: Clone your own repository, add code, commit, and push

Clone the repository.

Add a file `example.py` containing:

```python=
def add(a, b):
    return a + b

def subtract(a, b):
    return a + b  # do not change this line until prompted to do so.
```

Write a test function `def test_add()` for `add` to check that this function is working properly. Do NOT add a test function for `subtract` (yet).
Run pytest to ensure it works 

Then stage the file (`git add <filename>`), commit (`git commit -m "some commit message"`),
and push the changes (`git push`).


#### Step 3: Enable automated testing

In this step we will enable GitHub Actions.
- Select "Actions" from your GitHub repository page. You get to a page "Get started with GitHub Actions". 
- Select the button for "Set up this workflow" under Python Application.

![](https://i.imgur.com/7QOplAg.png)
Select “Python application” as the starter workflow.

GitHub creates the following file for you in the subfolder `.github/workflows`:


   ```yaml
# This workflow will install Python dependencies, run tests and lint with a single version of Python
# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions

name: Python application

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

jobs:
  build:

    runs-on: ubuntu-latest

    steps:
    - uses: actions/checkout@v2
    - name: Set up Python 3.9
      uses: actions/setup-python@v2
      with:
        python-version: 3.9
    - name: Install dependencies
      run: |
        python -m pip install --upgrade pip
        pip install flake8 pytest
        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
    - name: Lint with flake8
      run: |
        # stop the build if there are Python syntax errors or undefined names
        flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
        # exit-zero treats all errors as warnings. The GitHub editor is 127 chars wide
        flake8 . --count --exit-zero --max-complexity=10 --max-line-length=127 --statistics
    - name: Test with pytest
      run: |
        pytest
   ```

Replace `pytest` by `pytest example.py`:
```yaml
   - name: Test with pytest
     run: |
       pytest example.py
```
![](https://i.imgur.com/1TFZPRe.png)


Commit the change by pressing the "Start Commit" button.

#### Step 4: Verify that tests have been automatically run

Observe in the repository how the test succeeds. While the test is executing, the repository has a yellow marker.
This is replaced with a green check mark, once the test succeeds.

![](https://i.imgur.com/b8dI8XH.png)

Green check means passed.

Also browse the "Actions" tab and look at the steps there and their output.

#### Step 5: Add a test which reveals a problem

After you committed the workflow file, your GitHub repository will be ahead of your local cloned repository. Update your local cloned repository:

```
$ git pull origin main
```

Next uncomment add a test function `test_subtract` for to check that the `subtract` function can subtract two numbers from each other, and push it to your remote repository.
Verify that the test suite now fails on the “Actions” tab (GitHub).


#### Step 6: Open an issue on GitHub
Open a new issue in your repository about the broken test (click the “Issues” button on GitHub and write a title for the issue). The plan is that your colleague will fix the issue through a pull request

#### Step 7: Fork and clone the repository of your colleague

Fork the repository using the GitHub web interface. 
Make sure you clone the fork after you have forked it. Do not clone your colleague’s repository directly.


#### Step 8: Fix the broken test

Fix the function now and run pytest to check that it works.
Then push to _your fork_. Check whether the action now also passes.

#### Step 9: Open a pull request (GitHub)

Then before accepting the pull request from your colleague, observe how GitHub Actions automatically tested the code.

If you forgot to reference the issue number in the commit message, you can still add it to the pull request: `my pull request title, closes #NUMBEROFTHEISSUE`

#### Step 10

Observe how accepting the pull request automatically closes the issue (provided the commit message or the pull request contained the correct issue number).

Discuss whether this is a useful feature. And if it is, why do you think is it useful?

### Recap modular coding, documentation, Continuous Integration + collaborative Git + Github
* What questions do you still have?
* Whether there are any incremental improvements that can benefit your projects?
* What’s nice that we learnt but is overkill for your current work?

- I still have questions regarding testing, but that could be related to more advance topics. I feel that modularity will be very useful in my research. Probably packaging and unit testing are overkill for my current research.
- I think careful testing is important. I don't think that anything would be an overkill for >medium-importance projects
- I learned how to organize my own code although I still work alone, prviously I just use git add -A to dump everything into github and there is no organization and tracking. 
- I think the workshop was quite useful. I learned a lot about Github and how the projects are added there. How to keep the documentation. A little bit  more focus on modular coding would have been more beneficial. 
- I think from all the different aspects, at least the basics will be beneficial for my work. It is good to be aware of the possibilities, further evaluation will provide insights on what would be overkill or what will provide a better workflow going forward. 
- I will use the skills learnt from the workshop for my everyday codes for keeping tracks of all the changes and versions of my codes. Thanks for the good workshop.
- Writing more modular code and introducing tests is something that I will implement in my work. The git and shell theory and practice from Day 1 were also very useful. 


## 🧠 Collaborative Notes

Example test function:
```python!
	def add(a, b):
	    return a - b  # Uh oh, mistake! 😱
	 
	 
	def test_add():
	    assert add(2, 3) == 5
	    assert add('space', 'ship') == 'spaceship'
```

## 💬Feedback for the morning
Please give us some feedback about this morning, let us know one (or more) thing that went well and one thing that can be improved. This can be anything: the pace, the content, the relevance to your work, the interactiveness, how we answer questions. We use your feedback to tune the rest of the workshop to your needs! 

### What went well?

- The topic clearly described. The instructors are knowledgable.
- Important aspects of accomplishing a project are covered.
- Everything was explained clearly. The speed was good.
- Clear and complete examples + best practices on how to implement this ourselves. 
- I liked the modularization topic, it is engaging to encapsulate and structure the code. Also the readme advises were cool.
- Short slides, easy to follow, which is good.
### What can be improved?

- We could have more examples on the modular programming
- I think the modularization has some nice and more difficult topics that could be covered. For example, I ve seen the types of programming, when you first write the general architecture, then inside you write the logical steps and then for each step people write the piece of code that does it. I forgot the name, but i want to learn this type of software developement.
- I was hoping to learn documentation part with an exmple on how to use Sphinx.
- Hopefully we will learn packaging afternoon.
- 
- Examples from the real projects. 
- 
- More time and exercises for the modular rogramming.
- I think for this time frame things are OK, it would be great to have an advanced workshop afterwards!
- Perhaps more examples on modular programming
- How can we integrate bit with Python/MATLAB to run codes and make changes in real-time and update on repository. All from bit console.
- Try to complete the git and github part on the first day to have more time for the topics of the second day. 

## 📊 Post-workshop survey
Before you leave, please give us feedback on the workshop, by filling in the [post-workshop survey](
https://www.surveymonkey.com/r/VDDW3Y9)

## 📚 Resources

### Documentation:
- [Use Sphinx and Markdown to write user documentation](https://coderefinery.github.io/documentation/sphinx/)
- [Deploy Sphinx documentation to GitHub Pages](https://coderefinery.github.io/documentation/gh_workflow/)
- [Writing in Markdown on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Github Actions](https://docs.github.com/en/actions/learn-github-actions/understanding-github-actions)


### Testing
- [Testing in Matlab](https://nl.mathworks.com/help/matlab/matlab_prog/ways-to-write-unit-tests.html)


### Packaging
- [Creating a package with Poetry](https://carpentries-incubator.github.io/python-intermediate-development/43-software-release/index.html)

### Slides:
[Slides](https://lyashevska.github.io/ds-cr-slides/)
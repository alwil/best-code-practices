---
marp: true
title: "Code Quality"
paginate: false
theme: custom
backgroundColor: #fff

---
# Aspects of good quality code 
 
Today, you will review your code for

- Readability
- Reusability
- Robustness

![bg right:40% width:450](img/wtfs_per_minute_thumb.jpg)

---
# I. Code readability
#### Who is the audience that will read your code?

>Code is for computer, comments are for humans.

---
# Code readability

- ~~Code is for computer, comments are for humans.~~

- Use whitespace and newlines strategically.

---

#### Compare:

```python
if foo == 'blah': do_blah_thing()
do_one(); do_two(); do_three()
```
**with**
```python
if foo == 'blah':
    do_blah_thing()
do_one()
do_two()
do_three()
```

Compound statements are generally discouraged

---
# Code readability

- ~~Code is for computer, comments are for humans.~~

- Use whitespace and newlines strategically.

- use descriptive names for functions and variables
  - start functions with a verb
  - make variable names _just_ long enough to be meaningful

---
# Code readability
**Compare**

```r
for i in my_shopping_basket:
  if(test(i)) > 10:
    purch(i)
  else:
    disc(i)
```
**with**
```r
for item in basket:
  if(testNecessity(item)) > 10:
    purchase(item)
  else:
    discard(item)
```


---
# Code readability

- ~~Code is for computer, comments are for humans.~~

- Use whitespace and newlines strategically.

- use descriptive names for functions and variables
  - start functions with a verb
  - make variable names _just_ long enough to be meaningful

- use a consistent style 
  - consistency will make your code easier to understand and maintain
  - consult a styleguide for your language (keep conventions, and don't reinvent the wheel)
  
---
# Variable naming
Compare:

```python
myVar = original_variable + MOD(new.var)
```
with

```python
my_var = original_var + Modified(new_var)
```

_Are you using descriptive variables in your project?_


---
# Comments
- Comments that contradict the code are worse than no comments. Always make a priority of keeping the comments up-to-date when the code changes! 
- Ensure that your comments are clear and easily understandable to other speakers of the language you are writing in (ENGLISH!)
- Delete commented code 
- Inline comments are unnecessary and in fact distracting if they state the obvious. 

Don’t do this
```python
x = x + 1                 # Increment x
```
This is more useful
```python
x = x + 1                 # Compensate for border
```

---
# Styleguides

- Python style manual: [PEP-8](https://www.python.org/dev/peps/pep-0008/)
- MATLAB style guide: [MATLAB File-exchange](http://cnl.sogang.ac.kr/cnlab/lectures/programming/matlab/Richard_Johnson-MatlabStyle2_book.pdf)

![width:800](https://imgs.xkcd.com/comics/code_quality.png)
_Are you already following a style guide?_

---
# Your turn

#### Where can you improve the readability of your code?

- Run a linter (e.g. `flake8` for Python,`checkcode`/`mlint` for MATLAB, or `lintr` for R) to identify conflicts with style guides.
  
- If you find code that is hard to read, make a note to work on it.
(Schedule time to refactor, but do not do this now!)

_Tip! Use_ `#TODO` _or_ `//TODO` _(depending on your comment marker) to easily find these spots later on.
Many IDEs extract these into a task list (e.g. [MATLAB](https://blogs.mathworks.com/community/2008/03/17/whats-on-my-todo-list/))!_

---
#### Share your findings 
- Naming conventions
- Comments
- Formatting
- Compound statements
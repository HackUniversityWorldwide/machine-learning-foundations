## **Week 1 - Getting Started with Google Colab for Machine Learning**

## What this workshop is about
Week 1 is all about getting comfortable with the main tool we will use during the series: **Google Colab**.

Instead of starting with difficult machine learning theory, we start with the workspace where we will write code, take notes, and test ideas.

## Goal of this workshop
By the end of this session, participants will:
- know what Google Colab is
- create and run their first notebook cells
- understand the difference between **code cells** and **text cells**
- write a little Python inside Colab
- load a tiny dataset and look at it
- leave with a notebook they can keep building on later

## Why Google Colab?
Google Colab is a simple way to run Python in the browser.
It is a great beginner tool because:
- you do not need a heavy local setup to get started
- it mixes notes, code, and output in one place
- it is easy to save, share, and come back to later
- it is commonly used for data science and machine learning practice

## What we will do
1. Open Google Colab
2. Create a new notebook
3. Learn the basic interface
4. Run simple Python code
5. Add notes using Markdown
6. Import a library
7. Create a tiny table of data
8. Save and share the notebook

---

## Suggested session flow

### Part 1 — Open Google Colab
Create a **new notebook** and rename it to something simple like:

`week1_intro_colab.ipynb`

### First things to notice
- **Code cell** → where Python code runs
- **Text/Markdown cell** → where you write titles, notes, and explanations
- **Run button** → executes a cell
- **Runtime** → the environment where your code runs

---

### Part 2 — Run your first code cells
Try these one by one.

#### Example 1: Print text
```python
print("Hello, Colab!")
```

#### Example 2: Basic math
```python
2 + 3
```

#### Example 3: Variables
```python
name = "Your Name"
age = 20
print(name)
print(age)
```

#### Example 4: Tiny study example
```python
hours_studied = 2
pages_read = 15
print("Hours studied:", hours_studied)
print("Pages read:", pages_read)
```

---

### Part 3 — Add a text cell
Insert a **text cell** and write something like this:

```md
# My First Notebook
This is my first notebook in Google Colab.
Today I learned how to run code and write notes.
```

### Why this matters
In machine learning, notebooks are useful because you can:
- explain what you are doing
- write and test code
- show outputs and charts
- keep notes and experiments together

---

### Part 4 — Learn a few Python basics

#### Strings
```python
favorite_topic = "machine learning"
print(favorite_topic)
```

#### Numbers
```python
x = 10
y = 5
print(x + y)
print(x * y)
```

#### Lists
```python
numbers = [1, 2, 3, 4, 5]
print(numbers)
print(numbers[0])
```

#### Simple loop
```python
for n in numbers:
    print(n)
```

---

### Part 5 — Import a useful library
Now try importing a library:

```python
import pandas as pd
```

### What is pandas?
`pandas` helps us work with tables of data.
That is one of the most common things we do in machine learning.

---

### Part 6 — Create your first dataset
Copy and run this:

```python
import pandas as pd

data = {
    "Hours_Studied": [1, 2, 3, 4, 5],
    "Exam_Score": [50, 60, 65, 75, 90]
}

df = pd.DataFrame(data)
df
```

### What is happening here?
- we created a tiny dataset
- we turned it into a table
- Colab displays the table nicely

This is the kind of simple structure we will use later when learning how machine learning works.

---

### Part 7 — Explore the data a little
Try these commands:

```python
df.head()
```

```python
df.shape
```

```python
df.describe()
```

### Why this matters
Before building a machine learning model, we usually:
- look at the data
- understand what the columns mean
- check size and simple statistics

---

### Part 8 — Mini activity
Try changing the dataset.

#### Task ideas
- add one more student
- change the column names
- create a new dataset about sleep hours and mood
- print the average score

Example:

```python
print(df["Exam_Score"].mean())
```

---

### Part 9 — Save your work
At the end of the workshop:
- rename your notebook clearly
- save it to Google Drive
- optionally download it as `.ipynb`
- optionally upload it to GitHub later

Suggested file name:

`week1_intro_colab.ipynb`

## Suggested closing message
You do not need to know machine learning yet.
Today was about getting comfortable with the space where we will build everything else.

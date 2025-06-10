# git and github practice
## Task 1: Create a Repository for Your Project
Go to GitHub.

Click "New Repository".

Name it something like my-first-python-project.

Add:

- A description

- A README file (tick this)

- A Python .gitignore file

Click Create repository.
## Task 2: Open in GitHub Codespaces
On your new repo, click the green “<> Code” button.

Click "Codespaces" tab, then “Create codespace on main”.

This launches a full development environment in your browser.
## Task 3: Create a Python File and Run It
Inside Codespaces, in the left file panel:

Right-click → New File → name it hello.py.

Add this code:
``` python
print("Hello from Codespaces!")
```

Press Run or use the Terminal:
``` bash
python hello.py
```
##  Task 4: Create and Track Files with Git
Make a second file called about_me.py with some variables:

``` python
name = "Your Name"
age = 20
print(f"My name is {name} and I am {age} years old.")
```

Now track your changes:

``` bash
git add .
git commit -m "Add about_me.py"
git push
```
## Task 5: Edit a File and Make Another Commit
Go back to hello.py and change the message.

Add a second line of code.

Then commit again:

``` bash
git add hello.py
git commit -m "Updated hello message"
git push
```
## Task 6: Create a New Branch
Create a new branch in Terminal:

``` bash
git checkout -b experimenting
```

Create a new file, e.g., calculator.py and write a simple sum:

``` python
print(10 + 5)
```

Commit and push:

``` bash
git add .
git commit -m "Added calculator script"
git push --set-upstream origin experimenting
```
## Task 7: Use the Git Graph (Visualise Commits)
In Codespaces, open the Source Control panel (left bar).

Explore the timeline of your commits and branches.

Note how each file changed over time.
## Task 8: Explore the Terminal
Use basic terminal commands:

```bash
ls           # lists files
cd folder    # move into a folder
mkdir test   # create a new folder
rm filename  # delete a file
```
Optional: try editing files in the terminal using nano:

```bash
nano hello.py
```
### Task 9: Create a .gitignore File
Create a .gitignore file and add:

```markdown
*.log
*.csv
__pycache__/
```
Save it, and make a commit:

```bash
git add .gitignore
git commit -m "Add gitignore"
git push
```
## Task 10: Use Markdown in the README
Open the README.md file.

Add:

``` markdown
## About This Project
This is a sample Python project I'm building in GitHub Codespaces.

### Files
- `hello.py` – prints a welcome message
- `about_me.py` – prints your name and age
- `calculator.py` – does simple maths
```

Commit your changes:

```bash
git add README.md
git commit -m "Update README with project info"
git push
```
## Extensions

**Task 11:** Use input() to get user input in a Python file.

**Task 12:** Create a functions.py and define multiple reusable functions.

**Task 13:** Start working on a project (e.g. a calculator or simple data analysis script using lists).

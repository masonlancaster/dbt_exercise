# GitHub & Git Basics Lab

## Objective

In this lab you will:

- Create a GitHub account  
- Install VS Code and Git  
- Use the VS Code terminal  
- Clone a public GitHub repository  
- Create your own repository  
- Make changes locally  
- Commit and push changes from your own repo  

---

## Part 1 – Create a GitHub Account

1. Go to https://github.com  
2. Click **Sign up**  
3. Create a free account  
4. Verify your email  

---

## Part 2 – Install Visual Studio Code

### macOS

1. Go to https://code.visualstudio.com  
2. Download for Mac  
3. Open the `.dmg` file  
4. Drag VS Code to Applications  

### Windows

1. Go to https://code.visualstudio.com  
2. Download for Windows  
3. Run the installer  
4. Accept default options  

---

## Part 3 – Install Git

### macOS

1. Open VS Code  
2. Go to **Terminal → New Terminal**  
3. Run: ```git –version```

4. If Git is not installed, macOS will prompt you to install it.

If needed, download from:  
https://git-scm.com/download/mac

---

### Windows

1. Go to https://git-scm.com/download/win  
2. Download and run the installer  
3. Accept default settings  

After installing Git:

1. Open VS Code  
2. Go to **Terminal → New Terminal**  
3. Run: ```git –version```

---

## Part 4 – Configure Git

In VS Code:

**Terminal → New Terminal**

Run: 
```
git config –global user.name “Your Name”
git config –global user.email “your_email@example.com”
```

Use the same email as your GitHub account.

---

## Part 5 – Clone a Public Repository

We will clone a popular open-source repository: **freeCodeCamp**

Repository URL: ```https://github.com/freeCodeCamp/freeCodeCamp.git```

In the VS Code terminal: 
```
cd Desktop
git clone https://github.com/freeCodeCamp/freeCodeCamp.git
cd freeCodeCamp
code .
```

You now have a local copy of the repository.

(No changes are required for this repo.)

---

## Part 6 – Create Your Own Repository

### On GitHub

1. Go to https://github.com  
2. Click + → New repository  
3. Name the repository: ```intro-git-lab```

4. Set to Public  
5. Check "Add a README file"  
6. Click Create repository  

---

## Part 7 – Clone Your Repository

Copy the HTTPS link from your new repository.

In the VS Code terminal:
```
cd Desktop
git clone YOUR_REPO_URL
cd intro-git-lab
code .
```

---
---

## Part 8 – Create a New Branch

Before making any changes, create a new branch.

In the VS Code terminal: ```git checkout -b add-readme-content```

This creates a branch named `add-readme-content` and switches to it.

Check your branch: ```git branch```

The current branch will have a * next to it.

---

## Part 9 – Make a Change

Open `README.md` in VS Code and add:
```
##Intro Git Lab

This repository was created by Your Name.

This is my first GitHub project.
```

Save the file.

---

## Part 10 – Commit and Push to Your Branch

Stage files: ```git add .```

Commit: ```git commit -m “added content to readme”```

Push your branch to GitHub: ```git push -u origin add-readme-content```

---

## Part 11 – Create a Pull Request

1. Go to your repository on GitHub  
2. You should see a message about your recently pushed branch  
3. Click **Compare & pull request**

OR

1. Click the **Pull requests** tab  
2. Click **New pull request**  
3. Select:
   - Base branch: `main`
   - Compare branch: `add-readme-content`

4. Click **Create pull request**

---

## Part 12 – Add a Comment and Merge

1. In the pull request page, write a short comment such as:
```
Added introductory content to README file.
```

2. Click **Merge pull request**  
3. Click **Confirm merge**

Your changes are now merged into the main branch.

---

## Part 13 – Pull Latest Changes Locally (Optional)

Back in VS Code terminal:

```
git checkout main
git pull
```

This updates your local main branch with the merged changes.

---

## How Branches and Pull Requests Work

### What is a Branch?

A branch is a separate version of the code.

- The `main` branch usually contains the official, stable code which runs in production 
- New work is done in separate branches  

This allows people to:

- Work without breaking main code  
- Test changes safely  
- Work in parallel with others  

Example:

- main → production-ready code  
- feature-login → new login feature  
- bugfix-header → fix a bug  

---

### What is a Pull Request (PR)?

A pull request is a request to:

👉 Merge changes from one branch into another (usually into `main`)

It allows:

- Code review  
- Discussion  
- Testing before merging  

---

## How This Works in a Team Workflow

In a real software or data engineering team:

1. A developer creates a branch for a task  ```git checkout -b feature-new-report```

2. They make changes and commit them  

3. They push the branch to GitHub  

4. They open a pull request  

5. Teammates review the code and leave comments  

6. Once approved, the PR is merged into main  

---

### Why Teams Use This Process

✅ Prevents breaking production code  
✅ Encourages collaboration  
✅ Keeps history organized  
✅ Allows review and quality control  

---

## Submission

Submit:

- Link to your GitHub repository  
- Screenshot of your merged pull request
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

## Part 8 – Make a Change

Open `README.md` in VS Code and add:
```
##Intro Git Lab

This repository was created by Your Name.

This is my first GitHub project.
```

Save the file.

---

## Part 9 – Commit and Push

In the VS Code terminal: 
```
git add .
git commit -m “updated readme”
git push
```

---

## Submission

Submit:

- The link to your GitHub repository



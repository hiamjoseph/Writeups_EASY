# Collaborative Development

**Category:** General Skills  
**Difficulty:** Easy  
**Source:**
[picoCTF_COLLABORATIVE_DEVELOPMENT](https://play.picoctf.org/practice/challenge/410?page=2)  
**Date Solved:** 2024-08-20

## 📁 Description

> My team has been working very hard on new features for our flag printing
> program! I wonder how they'll work together?

## ✅ Solution

Merge all the git branches.

Execute the python file.

### 🧠 Approach

Collabration in development is usuall done through branching your project.

Teams merge their branches into the main branch, and see if there are any
conflicts that need to be resolved.

The same will happen in this challenge.

I personally inspected each branch with git-lens, a VS code tool, and combined
the text to get the flag.

### 💻 Commands

```bash
git branch -a
git merge <branch-name>
python3 <filename>
```

### ✌🏾 Additional tips

Use git-lens, it'a visual representaion of your git commits, branches and more.

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURnt0M0BtdzBya19tQGszc190aDNfZHIzQG1fdzBya19lNGI3OWVmYn0NCg==

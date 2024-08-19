# Commitment Issues

**Category:** General Skills  
**Difficulty:** Easy  
**Source:**
[picoCTF_COMMITMENT_ISSUES](https://play.picoctf.org/practice/challenge/411?page=2)  
**Date Solved:** 2024-08-19

## 📁 Description

> I accidentally wrote the flag down. Good thing I deleted it!

## ✅ Solution

Use a git command to go back a commit from your current state.

I used `git revert <branch-hash>`.

Save the file, and the flag is yours.

### 🧠 Approach

When i read commitment issues, i instantly thought of git commits.

And obviously the flag was in the `message.txt` file since there's a comment
saying `remove sensitive info`.

That's your flag.

### 💻 Commands

```bash
git log
git reset <branch-hash>
cat message.txt
```

### ✌🏾 Additional tips

Understand git,i it'll make your life easier.

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURntzQG4xdDF6M185NTM5YmU2Yn0=

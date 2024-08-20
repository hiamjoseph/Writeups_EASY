# CanYouSee

**Category:** Forensics  
**Difficulty:** Easy  
**Source:**
[picoCTF_canyousee](https://play.picoctf.org/practice/challenge/408?page=2)  
**Date Solved:** 2024-08-20

## 📁 Description

> How about some hide and seek?

## ✅ Solution

Display the metadata of the image.

Look under: `Attribution URL`, there's an encoded text.

Decode it and the flag is yours.

### 🧠 Approach

I personaly used `exiftool` to display the metadata.

### 💻 Commands

If you're on Mac

```bash
brew install exiftool
exiftool <imgname>
```

### ✌🏾 Additional tips

Look up other tools to show you more in-depth infos about your files.

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURntNRTc0RDQ3QV9ISUREM05fM2I5MjA5YTJ9Cg==

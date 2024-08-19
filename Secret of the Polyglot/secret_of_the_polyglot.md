# Secret of the Polyglot

**Category:** Forensics  
**Difficulty:** Easy  
**Source:**
[picoCTF_SECRET_OF_THE_POLYGLOT](https://play.picoctf.org/practice/challenge/423)  
**Date Solved:** 2024-08-13

## 📁 Description

> The Network Operations Center (NOC) of your local institution picked up a
> suspicious file, they're getting conflicting information on what type of file
> it is. They've brought you in as an external expert to examine the file. Can
> you extract all the information from this strange file?

## ✅ Solution

Change the extension of the `pdf` file to `png`.

Combine both contents to get the flag.

### 🧠 Approach

Check the content of the first file, it contains the second part of the flag;
save it somewhere.

Convert the file to a png image, open it and you'll se the first part of the
flag.

### 💻 Commands

Why did i convert to png?

run

```bash
file <filename>
```

You'll see that the actual file type is `png`

### ✌🏾 Additional tips

You can `cat` pdf files (i didn't know that)

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURntmMXUzbjdfMW5fcG45XyZfcGRmXzdmOWJjY2QxfQ==

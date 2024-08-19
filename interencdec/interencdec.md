# interencdec

**Category:** Cryptography  
**Difficulty:** Easy  
**Source:**
[picoCTF_INTERENCDEC](https://play.picoctf.org/practice/challenge/418)  
**Date Solved:** 2024-08-12

## 📁 Description

> Can you get the real meaning from this file.

## ✅ Solution

Decode the file with `BASE64`

remove the `b'` at the beginning.

Decode the result with the `caeser cipher`, try different ciphers till you get
the flag.

### 🧠 Approach

Use the command `base64 -d <filename>` to decode the file.

Remove any leading `b'` or trailing quotes from the decoded output.

Apply a Caesar cipher to the cleaned output. Try different shifts until the flag
is revealed.

### 💻 Commands

`base64 -d <filename>`

### ✌🏾 Additional tips

The ceaser cipher may differ for each user, for me it was `-19`

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURntjYWVzYXJfZDNjcjlwdDNkXzg5MGQyMzc5fQ==

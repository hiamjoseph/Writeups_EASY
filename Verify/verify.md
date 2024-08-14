# Verify

**Category:** Forensics  
**Difficulty:** Easy  
**Source:** [picoCTF_VERIFY](https://play.picoctf.org/practice/challenge/450)  
**Date Solved:** 2024-08-10

## 📁 Description

The goal of the challenge is to use the SHA-256 hashing function to check which
file is legitimate, hence containing the real flag.

## ✅ Solution

The file to be decrypted is _e018b574_. It contains the flag.

### 🧠 Approach

The _challenge.zip_ contains a _checksum.txt_ file; it contains a SHA-256 hash.
You can either use the `sha256sum *` in your 'files' folder command to display
all the hashes for the files. Decrypt the one with the same hash in the
_checksum.txt_ file.

---

OR

Write a sript to automate the check.

<!-- ### Exploits

Detail the steps and commands used to exploit the challenge. -->

### 💻 Commands

```bash
sha256sum <filename>
```

```bash
./decrypt.sh files/e018b574
```

### ✌🏾 Additional tips

If you get a `error at newline` error, use the built-in webshell. Don't try to
debug the _decrypt.sh_ file.

### ⛳️ The flag (BASE64 encrypted)

**PLEASE DON'T COPY PASTE**

cGljb0NURnt0cnVzdF9idXRfdmVyaWZ5X2UwMThiNTc0fQ==

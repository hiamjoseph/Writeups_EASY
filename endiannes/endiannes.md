# endiannes

**Category:** General Skills  
**Difficulty:** Easy  
**Source:**
[picoCTF_ENDIANNES](https://play.picoctf.org/practice/challenge/414?page=2)  
**Date Solved:** 2024-08-19

## 📁 Description

> Know of little and big endian?

## ✅ Solution

Convert the given string to ASCII and then to its HEX value, reverse the digits,
and convert to decimal, that's your little endian.

## Don't reverse the digits and that's your big endian.

## orrrrrrr

just do what i did.

### 🧠 Approach

When i started this challenge, i was clueless about endianess, i did a little
reading and the concept is quite simple.

Convert a string to its endian rep, you do the steps above; so far so good, i
understood that, but left out all the conversions, so all i did was reverse the
actual string; obviously, it didn't work.

So iiii got all lazy annnnnd.

With the little knowledge of the C language i had, i inspected the code, and saw
that both the `little_endian` and the `big_endian` were generated in your local
machine.

All i did was print them out at runtime.

### 💻 Commands

compile the source code with

```bash
gcc flag.c
```

### ✌🏾 Additional tips

Learn C, it'll make your life easier

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURnszbmRpNG5fc3c0cF9zdTMzZXNzXzI1YzVmMDgzfQ==

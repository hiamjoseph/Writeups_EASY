# Heap 0

**Category:** Binary Exploitation **Difficulty:** Easy  
**Source:** [picoCTF_Heap_0](https://play.picoctf.org/practice/challenge/438)  
**Date Solved:** 2024-08-10

## 📁 Description

> Are overflows just a stack concern?

Use your C knowledge to solve this challenge.

## ✅ Solution

Write a 17 byte string to the input. NO SPACES.

### 🧠 Approach

The key to solving this challenge is reading the source code.

Upon close inspection of the code, you'll find that `scanf()` in the
`writet_buffer` function isn't inside any `if` checks, in other words, it's not
properly validated.

Our two variables addresses are `0x6000035b0030` and `0x6000035b0040`. The
difference is `0x10` or 16 in decimal.

This time, choose the second option of writing to the buffer.

Input any string that's longer than 16 bytes, and the flag is yours.

### 💻 Commands

If you decide to only use the source code, you'll have to compile the program
yourself.

use `gcc <sourcecode>`

### ✌🏾 Additional tips

This challenge requires a good understanding of the C language. Dynamic memory
allocation and pointers.

### ⛳️ The flag (BASE64 encoded)

**PLEASE DON'T COPY PASTE**

cGljb0NURntteV9maXJzdF9oZWFwX292ZXJmbG93X2MzOTM1YTA4fQ==

# Unminify

**Category:** Web Exploitation  
**Difficulty:** Easy  
**Source:**
[picoCTF_UNMINIFY](https://play.picoctf.org/practice/challenge/426)  
**Date Solved:** 2024-08-09

## 📁 Description

> I don't like scrolling down to read the code of my website, so I've squished
> it. As a bonus, my pages load faster!

## ✅ Solution

Inspect the page.

With your understanding of HTML; navigate to

```html
`
<body>
  <center>
    <div>
      <div>
        <div> <p class="THE FLAAAAAG"></p> </div>
      </div>
    </div>
  </center>
</body>
```

### 🧠 Approach

There's a hidden `<p>` tag in the markup, look for it.

### 💻 Commands

NO COMMANDS WERE USED.

### ✌🏾 Additional tips

A liitle bit of HTML wouldn't hurt.

### ⛳️ The flag (BASE64 encrypted)

**PLEASE DON'T COPY PASTE**

cGljb0NURntwcjN0dHlfYzBkM181MWQzNzRmMH0=

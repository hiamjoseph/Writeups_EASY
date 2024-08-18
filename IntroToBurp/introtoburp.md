# IntroToBurp

**Category:** Web Exploitation  
**Difficulty:** Easy  
**Source:**
[picoCTF_INTROTOBURP](https://play.picoctf.org/practice/challenge/419)  
**Date Solved:** 2024-08-18

## 📁 Description

> Additional details will be available after launching your challenge instance.

## ✅ Solution

Use Burp to intercept the Requests made from the website.

Keep submitting forms until your reach the 2FO; input anything into it.

Upon submission, a `otp = <your code here>` will appear in Burp; delete it and
forward the request.

The flag will appear in the browser.

### 🧠 Approach

Open Burp Suite and ensure that the "Intercept is on" in the "Proxy" >
"Intercept" tab.

Use Burp's embedded browser.

Start filling out and submitting forms on the website as usual. Continue this
process until you reach the specific form labeled 2FO.

On the 2FO form, input any value into the fields. The actual data you enter
doesn't matter, as the focus is on intercepting the submission.

Upon submitting the 2FO form, the request will be intercepted by Burp Suite.

Look for the portion of the intercepted request that includes
`otp = <your code here>`.

Delete the otp parameter and its value entirely from the request.

After deleting the otp parameter, click "Forward" to send the modified request
to the server.

### 💻 Commands

NO COMMANDS WERE USED.

### ✌🏾 Additional tips

Burp suite can be a little confusing at first, just make sure you download the
right version; Burp Community edition, it's more than enough for this challenge
and pretty powerful for other things too.

### ⛳️ The flag (BASE64 encrypted)

**PLEASE DON'T COPY PASTE**

cGljb0NURnsjMFRQX0J5cHZzc19TdUNjMyRTX2M5NGI2MWFjfQ==

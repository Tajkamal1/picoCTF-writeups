# 🧠 picoCTF – Bookmarklet Writeup

## 📌 Challenge Information
- **Name:** Bookmarklet  
- **Category:** Web Exploitation  
- **Author:** Jeffery John  

---

## 📝 Description
The challenge provides a web page where a flag can be revealed using a **JavaScript bookmarklet**. The goal is to execute JavaScript in the browser console to reveal the hidden flag.

---

## 🎯 Objective
- Explore the web page  
- Use the provided JavaScript in the console  
- Extract the hidden flag  

---

## 🔍 Methodology
- Opened the web page and read the instructions  
- Inspected the page source using browser Developer Tools  
- Found JavaScript code that prints the flag  
- ![JavaScript code in page source](https://github.com/user-attachments/assets/24fa3b7a-68fd-477e-bb83-eea9daf0210f)  
- Prepared to execute the JavaScript in the browser console  

---

## 🚨 Exploitation
- ➤ Open **Developer Tools** in your browser (`F12` or `Ctrl + Shift + I`)  
- ➤ Go to the **Console** tab  
- ➤ Click on the **blinking cursor** in the console  
- ➤ **Right-click** → Select **“Paste”**  
- ➤ Paste the JavaScript code you found in the page source  
- ➤ Press **Enter** to execute the code  
- ➤ The flag will be printed directly in the console  
- ![Flag printed in console](https://github.com/user-attachments/assets/d0cca052-4011-4335-a81f-802b08106994)  

---

## 🏁 FlagpicoCTF{p@g3_turn3r_e8b2d43b}

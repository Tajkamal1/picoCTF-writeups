# 🧠 picoCTF – GET aHEAD Writeup

## 📌 Challenge Information
- **Name:** GET aHEAD  
- **Category:** Web Exploitation  
- **Author:** madStacks  

---

## 📝 Problem Statement
The challenge provides a web application with a clickable interface. The goal is to find the hidden flag stored on the server by analyzing and manipulating the HTTP requests sent when interacting with the application.

---

## 🎯 Objective
- Identify the request triggered by the web page button  
- Intercept and analyze HTTP traffic  
- Modify the request to access hidden resources  
- Retrieve the flag from the server response  

---

## 🔍 Procedure Followed
1. Opened the challenge website: `http://wily-courier.picoctf.net:51989/`
<img width="1918" height="1021" alt="Screenshot 2026-03-18 130414" src="https://github.com/user-attachments/assets/d2313545-b897-4a4c-810b-cacf66d97691" />
2. Observed a **blue button** on the page, which likely triggers a request to the server  
3. Launched **Burp Suite** and enabled the Proxy to intercept HTTP requests  
4. Clicked the blue button and captured the **POST request** in the Proxy tab  
<img width="1897" height="1002" alt="Screenshot 2026-03-18 130927" src="https://github.com/user-attachments/assets/8d9f3966-7c0d-4561-b1ec-7dd6a4530624" />
5. Sent the captured request to **Repeater** (`Ctrl + R`) to analyze it further 
<img width="1895" height="1003" alt="Screenshot 2026-03-18 130853" src="https://github.com/user-attachments/assets/6e40c3ab-b92f-4497-94e2-1fbd0588db53" />

<img width="1899" height="1007" alt="Screenshot 2026-03-18 130958" src="https://github.com/user-attachments/assets/1d4e6ded-4fc2-4fbc-9a52-c35e801742b0" />
picoCTF{r3j3ct_th3_du4l1ty_8b13f07}
6. Examined the request and response to understand server behavior  
7. Modified the request path to access a sensitive file directly:  

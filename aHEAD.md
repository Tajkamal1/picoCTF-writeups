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

1. Opened the challenge website:  
   `http://wily-courier.picoctf.net:51989/`  

   ![Website Interface](https://github.com/user-attachments/assets/d2313545-b897-4a4c-810b-cacf66d97691)

2. Observed a **blue button** on the page, which triggers a request to the server  

3. Launched **Burp Suite** and enabled Proxy to intercept HTTP requests  

4. Clicked the blue button and captured the **POST request** in Burp Proxy  

   ![Captured POST Request](https://github.com/user-attachments/assets/8d9f3966-7c0d-4561-b1ec-7dd6a4530624)

5. Sent the captured request to **Repeater** (`Ctrl + R`) for further analysis  

   ![Request in Repeater](https://github.com/user-attachments/assets/6e40c3ab-b92f-4497-94e2-1fbd0588db53)

6. Analyzed the request and response behavior  

7. Modified the request path to access a sensitive file:
/flag.txt


8. Sent the modified request using Repeater  

   ![Flag Response](https://github.com/user-attachments/assets/1d4e6ded-4fc2-4fbc-9a52-c35e801742b0)

9. Successfully retrieved the flag from the response  

---

## 🏁 Flag

picoCTF{r3j3ct_th3_du4l1ty_8b13f07}















                                                                    

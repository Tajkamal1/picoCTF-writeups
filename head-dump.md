# 🧠 picoCTF – head-dump Writeup

## 📌 Challenge Information
- **Name:** head-dump  
- **Category:** Web Exploitation  
- **Author:** Prince Niyonshuti N.  

---

## 📝 Description
A blog-based web application (picoCTF News) contains hidden functionality. The objective is to identify an exposed endpoint leaking server memory and retrieve the flag.

---

## 🎯 Objective
- Locate a vulnerable endpoint  
- Access the server memory dump  
- Extract the hidden flag  

---

## 🔍 Methodology
- Analyzed the web application interface and explored all available pages  
- Identified an **API Documentation** link
- <img width="1918" height="968" alt="image" src="https://github.com/user-attachments/assets/673f7fac-38df-419b-b940-47cb9368ddaf" />
- Navigated to the API documentation page  
- Inspected available endpoints  
- Found a heap dump endpoint  

---

## 🚨 Exploitation
- Selected the heap dump endpoint  
- Executed the request via the interface  
- Downloaded the memory dump file  
- Extracted the flag from the file  

---

## 🏁 Flag

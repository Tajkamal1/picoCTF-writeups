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
- <img width="1918" height="973" alt="image" src="https://github.com/user-attachments/assets/24dca618-2a2c-4d33-bfda-b07896908f05" />


---

## 🚨 Exploitation
- Selected the heap dump endpoint  
- Executed the request via the interface  
- Downloaded the memory dump file
- <img width="1918" height="968" alt="image" src="https://github.com/user-attachments/assets/a16c93ec-ca3d-4d95-96aa-55071f36f7a5" />
- Extracted the flag from the file
- <img width="1918" height="1022" alt="image" src="https://github.com/user-attachments/assets/f403dbd1-ca24-4e4c-ae5f-a4cda1762fb7" />


---

## 🏁 Flag

picoCTF{Pat!3nt_15_Th3_K3y_dc0756a3}


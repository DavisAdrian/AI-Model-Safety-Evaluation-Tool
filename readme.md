
---

# **🔐 Web Application Vulnerability Assessment of OWASP Juice Shop**

> A comprehensive **web application vulnerability assessment** performed on **OWASP Juice Shop**, an intentionally vulnerable e-commerce platform, using industry-standard tools like **OWASP ZAP**, **Burp Suite**, and **Nikto**.
>
>This project identifies **real-world security flaws** mapped to the **OWASP Top 10**, demonstrates exploitation techniques, and provides **secure coding solutions** in **Node.js/TypeScript** to remediate each vulnerability. The assessment highlights how common security gaps — like **SQL Injection**, **Broken Access Control**, **Directory Traversal**, and **Business Logic Flaws** — can lead to severe business and data breaches if left unaddressed.

---

## **📌 Project Files**

* [Overview](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-overview)
* [Objectives](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-vulnerabilities-demonstrated)
* [Tools & Technologies](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-tools--technologies)
* [Vulnerabilities Demonstrated](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-vulnerabilities-demonstrated)
* [Secure Coding Fixes](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-secure-coding-fixes)
* [Project Files](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-project-files-1)
* [How to Run Juice Shop Locally](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#%EF%B8%8F-how-to-run-juice-shop-locally)
* [Team Members](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-team-members)
* [Key Takeaways](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/readme.md#-key-takeaways)

---

## **📖 Overview**

This project demonstrates a **complete security assessment lifecycle**:

1. Setting up a **virtualized testing environment**
2. Scanning OWASP Juice Shop with **ZAP**, **Burp Suite**, and **Nikto**
3. Performing **manual testing** to identify additional flaws
4. Mapping vulnerabilities to the **OWASP Top 10**
5. Providing **secure coding fixes** in **TypeScript/Node.js**
6. Delivering findings in a **final report** and **presentation**

---

## **🎯 Objectives**

* Perform a vulnerability assessment on **OWASP Juice Shop**.
* Identify and demonstrate **3–5 critical vulnerabilities**.
* Show **business impact** and exploitation methodology.
* Provide **secure coding practices** for remediation.
* Present results in a **comprehensive report** and **live demo**.

---

## **🛠 Tools & Technologies**

| Tool / Technology          | Purpose                             |
| -------------------------- | ----------------------------------- |
| **OWASP Juice Shop**       | Target vulnerable web app           |
| **OWASP ZAP**              | Automated scanning & spidering      |
| **Burp Suite**             | Proxy testing & manual exploitation |
| **Nikto**                  | Web server vulnerability checks     |
| **Node.js + TypeScript**   | Understanding application internals |
| **Express.js**             | Backend secure coding fixes         |
| **Kali Linux / Ubuntu VM** | Testing environment                 |

---

## **🚨 Vulnerabilities Demonstrated**

| Vulnerability             | OWASP Category          | Impact                              | Demo Location |
| ------------------------- | ----------------------- | ------------------------------      | ------------- |
| **SQL Injection**         | Injection               | Admin login bypass, data theft      | `/login`      |
| **Broken Access Control** | IDOR                    | Access other users’ shopping carts  | `/user/:id`   |
| **Directory Traversal**   | Sensitive Data Exposure | Access confidential documents       | `/ftp/`       |
| **Bully Chatbot**         | Business Logic Flaw     | Exploit discount system             |  `/chatbot`    |

---

## **💻 Secure Coding Fixes**

Each vulnerability includes **insecure vs. secure code** examples in **TypeScript/Node.js**.

* **SQL Injection** → Use **parameterized queries** & hashed passwords
* **Broken Access Control** → Implement **server-side authorization**
* **Directory Traversal** → Restrict file paths & enforce authentication
* **Bully Chatbot** → Add **rate-limiting & input validation**

---

## **📂 Project Files**

* 📄 [Final Report](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/TTPR%20Capstone%20Report.pdf)
* 🛠️ [Secure Coding Review](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/secure%20coding%20Review/Security%20Fixes%20Summary.md)
* 🖼️ [Presentation Slides](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/Capstone%20Project%20Presentation%20.pdf)
* 🔍 [ZAP Scan Results](https://github.com/DavisAdrian/Owasp-Juice-shop-vulnerablilties-assessment/blob/main/Aiden's%20Final%20Capstone%20Report.pdf)

---

## **▶️ How to Run Juice Shop Locally**

```bash
# Clone Juice Shop
git clone https://github.com/juice-shop/juice-shop.git
cd juice-shop

# Install dependencies
npm install

# Start the app
npm start

# Open in browser
http://localhost:3000
```

---

## **👥 Team Members**

| Name       | Role                              |
| ---------- | --------------------------------- |
| **Adrian Davis** | Secure Coding & Remediation Lead  |
| **Kairos Liang** | Vulnerability Scanning Specialist & Data Analytics |
| **Aiden Yeung**  | Vulnerability Scanning Specialist & Impact Analysis|

---

## **🌟 Key Takeaways**

* Security testing is critical to protecting sensitive data.
* Automated tools + manual verification = **stronger coverage**.
* Mapping vulnerabilities to **secure coding practices** bridges the gap between finding and fixing flaws.

---

*This project is for educational purposes only and demonstrates defensive security techniques to help developers identify and fix vulnerabilities in web applications.*

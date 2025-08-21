
---

# **🔐 Web Application Vulnerability Assessment of OWASP Juice Shop**

> A comprehensive **web application vulnerability assessment** performed on **OWASP Juice Shop**, an intentionally vulnerable e-commerce platform, using industry-standard tools like **OWASP ZAP**, **Burp Suite**, and **Nikto**.
>
>This project identifies **real-world security flaws** mapped to the **OWASP Top 10**, demonstrates exploitation techniques, and provides **secure coding solutions** in **Node.js/TypeScript** to remediate each vulnerability. The assessment highlights how common security gaps — like **SQL Injection**, **Broken Access Control**, **Directory Traversal**, and **Business Logic Flaws** — can lead to severe business and data breaches if left unaddressed.

---

## **📌 Project Files**

* [Overview](#overview)
* [Objectives](#objectives)
* [Tools & Technologies](#tools--technologies)
* [Vulnerabilities Demonstrated](#vulnerabilities-demonstrated)
* [Secure Coding Fixes](#secure-coding-fixes)
* [Project Files](#project-files)
* [How to Run Juice Shop Locally](#how-to-run-juice-shop-locally)
* [Team Members](#team-members)
* [Screenshots](#screenshots)

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

📂 Check out: [`code-snippets/insecure_vs_secure_examples.ts`](./code-snippets/insecure_vs_secure_examples.ts)

---

## **📂 Project Files**

* 📄 [Final Report](./report/Capstone_Report.pdf)
* 🛠️ [Secure Coding Review](./report/Secure_Coding_Review.pdf)
* 🖼️ [Presentation Slides](./slides/Capstone_Presentation.pdf)
* 🔍 [ZAP Scan Results](./findings/zap_scan_results.pdf)

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
| **Aiden Yeung**          | Vulnerability Scanning Specialist & Impact Analysis|

---

## **📸 Screenshots** *(Optional, but highly recommended)*

Add screenshots of:

* Vulnerability exploitation
* Secure vs insecure code
* ZAP/Burp scan results
* Final Juice Shop interface

Example:

```markdown
![SQL Injection Demo](./images/screenshots/sql-injection-demo.png)
```

---

## **🌟 Key Takeaways**

* Security testing is critical to protecting sensitive data.
* Automated tools + manual verification = **stronger coverage**.
* Mapping vulnerabilities to **secure coding practices** bridges the gap between finding and fixing flaws.

---

## **📢 Next Steps**

* Upload your **reports, slides, and code snippets** to the repo.
* Add a few **screenshots** to make the README visually appealing.
* Pin the repo on GitHub for portfolio visibility.

---

*This project is for educational purposes only and demonstrates defensive security techniques to help developers identify and fix vulnerabilities in web applications.*

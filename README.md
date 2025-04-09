# codealpha_ task to create bug_bounty

Note :- No file/folder to upload as I did all things in Linux Terminal

# Bug Bounty Practice - DVWA XSS Task

This project is part of my bug bounty learning journey.  
I practiced finding vulnerabilities using **Burp Suite** and **DVWA (Damn Vulnerable Web Application)**.

---

## 🔧 Tools Used

- **Burp Suite** – For intercepting and modifying HTTP traffic
- **DVWA (Damn Vulnerable Web App)** – A local test site for practicing bugs
- **Docker** – To run DVWA easily on my computer
- **Firefox** – Web browser to interact with DVWA

---

## 🚀 What I Did

1. Installed DVWA using Docker:


2. Visited `http://localhost/setup.php` and clicked **Create / Reset Database**

3. Logged into DVWA with:
- Username: `admin`
- Password: `password`

4. Set DVWA Security Level to **Low**

5. Opened **XSS (Reflected)** section in DVWA

6. Entered the following test script:
```html
<script>alert('Hello!')</script>



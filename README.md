<div align="center">

# 🔐 Networkwalks – Week 3 Cybersecurity Internship Project

**W3-PM1: Password Cracking with JTR & W3-PM2: Password Cracking with NETWORKWALKS Tools**
</div>

---

## 📌 Project Overview

This project focuses on password cracking and helps develop Cybersecurity skills such as Ethical Hacking, Penetration Testing. It is made of two modules : Project Module 1 (PM1) and Project Module 2 (PM2). 

The purpose of PM1 is to use John The Ripper (JTR) in a Windows environment for password cracking. The PM2 aims to use two Networkwalks tools for password cracking.

The password-cracking activities presented in this project should only target authorized files and devices or those you own for security testing.

---

# 🔓 PM1 - Password Cracking with JTR

---

## ⚓ Background

John the Ripper (JTR) is a popular password cracking tool used by security professionals to test how strong
passwords are. It started as a tool for Unix systems but now works on Windows, Linux, and Mac. It can
check many types of password hashes and also unlock password protected files like PDF, ZIP, and Office
documents.

Johnny is the graphical version of John the Ripper. It gives a simple point and click screen, so beginners can
use JTR without typing long commands. Both tools are widely used in security testing and learning labs to
understand password safety.

In this lab task you will use JTR John and JTR Johnny to recover the password of a protected PDF file. This
exercise helps you learn how password cracking works and why it is important to use strong passwords for
protection.

---

## 🎯 Objective

The PM1's objective is to crack the password of attached PDF files using JTR JOHN and JTR JOHNNY tools on a Windows PC.

---

## 👣 Step 1

We downloaded John the Ripper (JTR) JOHN and Johnny GUI from the official websites on our windows PC.

---

![1_step_1.png](/screenshots/1_step_1.png)

---

## 👣 Step 2

We unzipped both downloaded JTR files.

We run the setup file of Johnny and installed it. We launched Jonny and set up the John The Ripper executable.

The executable file **john.exe** is located in the run folder: 

````text
/john-1.9.0-jumbo-1-win64/run/john.exe
````

---

![1_step_2.png](/screenshots/1_step_2.png)

---

## 👣 Step 3

We downloaded the locked pdf files from the Networkwalks project's Google Drive link. The downloaded files are available in **`/downloads`**.

---

### Getting the hash of PDF1

We open the hash website (Online HashCrack) in a browser.

We uploaded the file `/downloads/My Locked PDF1.pdf` and got its hash. We copied the hash and saved in the text file `/output_files/hash1.txt`. 

---

![1_step_3.png](/screenshots/1_step_3.png)

---

### Getting the password of PDF1

We opened Jonny and clicked on **Open password file**. We browsed to the saved *hash1.txt* file and clicked on **Open**.

---

![1_step_4.png](/screenshots/1_step_4.png)

---

We clicked on **Start new attack**. The PDF file password was cracked.

---

![1_step_5.png](/screenshots/1_step_5.png)

---

We exported and saved the password to `/output_files/password_1.txt` and `/output_files/password_1.csv`.

### Unlocking the PDF1 file

We opened the encrypted file `/downloads/My Locked PDF1.pdf` and entered the password we got **`good-luck`**.

---

![1_step_6.png](/screenshots/1_step_6.png)

---

We validated the password and the PDF file opened.

---

![1_step_7.png](/screenshots/1_step_7.png)

---

### Captured Flag

The captured flag is **`nw{cybersecurity_flag_captured_2608}`**.

---

![1_flag1.png](/screenshots/1_falg1.png)

---

## 🔂 Repeating step 3

We repeated the **step 3** for the two other encrypted PDF files **`/downloads/My Locked PDF2.pdf`** and **`/downloads/My Locked PDF3.pdf`**.

---

### Getting the hash of PDF2

We open the hash website (Online HashCrack) in a browser.

We uploaded the file `/downloads/My Locked PDF2.pdf` and got its hash. We copied the hash and saved in the text file `/output_files/hash2.txt`. 

---

### Getting the password of PDF2

We opened Jonny and clicked on **Open password file**. We browsed to the saved *hash2.txt* file and clicked on **Open**.

We clicked on **Start new attack**. The PDF file password was cracked.

---

![1_step_8.png](/screenshots/1_step_8.png)

---

We exported and saved the password to `/output_files/password_2.txt` and `/output_files/password_2.csv`.

### Unlocking the PDF2 file

We opened the encrypted file `/downloads/My Locked PDF2.pdf` and entered the password we got **`password1`**.

---

![1_step_9.png](/screenshots/1_step_9.png)

---

We validated the password and the PDF file opened.

---

![1_step_10.png](/screenshots/1_step_10.png)

---

### Captured Flag

The captured flag is **`nw{networkwalks_persistence_jtr_270521}`**.

---

![1_flag2.png](/screenshots/1_falg2.png)

---

### Getting the hash of PDF3

We open the hash website (Online HashCrack) in a browser.

We uploaded the file `/downloads/My Locked PDF3.pdf` and got its hash. We copied the hash and saved in the text file `/output_files/hash3.txt`. 

---

### Getting the password of PDF3

We opened Jonny and clicked on **Open password file**. We browsed to the saved *hash3.txt* file and clicked on **Open**.

We clicked on **Start new attack**. The PDF file password was cracked.

---

![1_step_11.png](/screenshots/1_step_11.png)

---

We exported and saved the password to `/output_files/password_3.txt` and `/output_files/password_3.csv`.

### Unlocking the PDF3 file

We opened the encrypted file `/downloads/My Locked PDF3.pdf` and entered the password we got **`1qaz2wsx`**.

---

![1_step_12.png](/screenshots/1_step_12.png)

---

We validated the password and the PDF file opened.

---

![1_step_13.png](/screenshots/1_step_13.png)

---

### Captured Flag

The captured flag is **`nw{networkwalks_flag_260821_1}`**.

---

![1_flag3.png](/screenshots/1_falg3.png)

---

# 🔓 PM2 - Password Cracking with Networkwalks Tools

---

## ⚓ Background

Password cracking is the process of recovering a password from stored data or a protected file. Security
professionals use it to test how strong a password is and to show why weak passwords are risky. If a
password is short or common, it can be found quickly, which proves the need for strong passwords.

Many files like PDF, ZIP, and Office documents can be locked with a password. When a file is locked, its
password is stored in the form of a hash. A hash is a scrambled value that represents the password. To
recover the password, we first take out this hash from the file, and then run it through a cracking tool that
tries different words until it finds a match.

In this lab you will use two free online tools made by Networkwalks. First you will use the Hash Calculator
to take the hash out of a locked PDF file. Then you will use the Password Cracker to find the real password
from that hash. Both tools run in your web browser, so you do not need to install anything.

This lab helps you understand how password cracking works step by step and why strong passwords are
important for protection.

---

## 🎯 Objective

The PM2's objective is to crack the password of the attached PDF file "My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf" using the Networkwalks Hash Calculator and Password Cracker tools on a Windows laptop.

---

## 👣 Step 1

We downloaded the encrypted PDF file **`My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf`** to our laptop from the Networkwalks project's Google Drive link. The downloaded file is available in **`/downloads/`**

---

![2_step_1.png](/screenshots/2_step_1.png)

---

## 👣 Step 2

We opened the Networkwalks Hash Calculator in our web browser.

---

![2_step_2.png](/screenshots/2_step_2.png)

---

## 👣 Step 3

We uploaded the downloaded locked PDF file to the Hash Calculator. And we got the hash value.

---

![2_step_3.png](/screenshots/2_step_3.png)

---

## 👣 Step 4

We copied the hash value given by the Networkwalks Hash Calculator tool.

---

## 👣 Step 5

We opened the Networkwalks Password Cracker in your web browser.

---

![2_step_5.png](/screenshots/2_step_5.png)

---

## 👣 Step 6

We pasted the hash value in the Password Cracker.

---

![2_step_6.png](/screenshots/2_step_6.png)

---

## 👣 Step 7

We started the attack. The tool tried different passwords until it found the match. The cracked password was shown on the screen.

---

![2_step_7.png](/screenshots/2_step_7.png)

---

We copied and saved the shown password in the txt file **`/output_files/password_4.txt`**.

---

## 👣 Step 8

We opened the locked PDF file and entered the cracked password **`password1`**.

---

![2_step_8.png](/screenshots/2_step_8.png)

---

## 👣 Step 9

We validated the entered password and the locked PDF file opened successfully.

---

![2_step_9.png](/screenshots/2_step_9.png)

---

### Captured Flag

The captured flag is **`nw{networkwalks_flag1_jtr_270521_1}`**.

---

![2_flag1.png](/screenshots/2_falg1.png)



# 💡 What I practiced

Through this project, I practiced password hacking with different tools. I cracked hashes and found the passwords to open locked pdf files. The abilities developed in these activities can be used to hack many other kinds of passwords, including credentials and wi-fi passwords. I tested the data security regarding their confidentiality. I captured the hidden flags. I used the popular Cybersecurity tool John The Ripper (JTR) in a Windows environment. I also experienced the Networkwalks Hash Calculator and Password Cracker tools.

I demonstrated Ethical Hacking and Data Security skills.

The most important skills I demonstrated include:

### 1. Password hacking

I used JTR and Networkwalks tools to hack the passwords and capture the flags. 

### 2. Catch The Flag

I captured the hidden flags and documented them faithfully.

### 3. Online HashCrack tool

I used the Online HashCrack tool to find the hash value of PDF files.

### 4. JTR tools

I used JTR tools to get the plain text passwords from hash values. 

### 5. Networkwalks tools

I used the Networkwalks Hash Calculator tool to find the hash value of a PDF file, and the Networkwalks Password Cracker tool to get the plain text password from the hash value.

### 6. Cyber Threat Intelligence 

By testing the strength of the passwords and the data security earlier, I demonstrated Cyber Threat Intelligence skills, including Threat Hunting and Threat Detection.

### 7. Intrusion Prevention (IPS)

By testing the strength of the passwords for data security and early detecting their weakness and related threats, I can enhance the security level and prevent an attacker from hacking the passwords. The PDF files might contain critical data like credentials, server details that could help an attacker to perform an intrusion.

### 8. Security-tool experimentation

Using different tools such as JTR John, JTR Johnny, as well as Networkwalks Hash Calculator and Passwrd Cracker tools to hack passwords is a practical way to experiment and master security tools.

### 9. Security mindset

A security mindset in cybersecurity is a proactive, analytical way of thinking. I demonstrated that mindset throughout this project by using appropriate tools and testing the strength of the passwords that were supposed to ensure data privacy.

### 10. Documentation

I documented tools, platforms links, screenshots, tasks and solutions. That is an important part of a professional cybersecurity project.

---

# 🔐 Security & Ethical Use

This project is intended strictly for education purposes only.

>>⚠️ Important: The skills demonstrated in this project must only be used on systems that you own or have explicit permission to test. Do not use the knowledge or the tools to attack unauthorized systems.

---

# 🔗 Tools & Resources

- **JTR John download:** [https://www.openwall.com/john/](https://www.openwall.com/john/)
- **JTR Johnny download:** [https://openwall.info/wiki/john/johnny](https://openwall.info/wiki/john/johnny)
- **Online HashCrack:** [https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php](https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php)
- **Networkwalks Hash Calculator:** [https://networkwalks.com/hash-calculator/](https://networkwalks.com/hash-calculator/)
- **Networkwalks Password Cracker:** [https://networkwalks.com/password-cracker/](https://networkwalks.com/password-cracker/)

---

# 👤 Author

**Syed Amaan Jaffri**\
Student of FAST University

LinkedIn: https://www.linkedin.com/in/syed-amaan-jaffri-571577291/

---

## 📌 Project Information

**Program Name:** Cybersecurity at Networkwalks | **Week:** 03 | **Project:** Password Hacking With JTR & Networkwalks Tools | **Repository:** GitHub


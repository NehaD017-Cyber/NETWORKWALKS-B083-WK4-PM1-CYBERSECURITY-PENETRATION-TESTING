# NETWORKWALKS-B083-WK4-PM1-CYBERSECURITY-PENETRATION-TESTING-AND-VULNERABILITY-ASSESSMENT

---

A comprehensive hands-on penetration testing project evaluating the security posture of Mediroza General Hospital. Covers target reconnaissance, vulnerability assessment, initial system access, credential cracking, and a final risk remediation report.

---

<!-- Core Domain & Tools -->
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-000000?style=for-the-badge&logo=cyberdefenders&logoColor=white)
![Penetration Testing](https://img.shields.io/badge/Penetration_Testing-FF0000?style=for-the-badge&logo=kalilinux&logoColor=white)
![Ethical Hacking](https://img.shields.io/badge/Ethical_Hacking-00599C?style=for-the-badge&logo=securityscorecard&logoColor=white)
![Vulnerability Assessment](https://img.shields.io/badge/Vulnerability_Assessment-4A154B?style=for-the-badge&logo=databricks&logoColor=white)

<!-- Environment & Utilities -->
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C93?style=for-the-badge&logo=kalilinux&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white)
![Nmap](https://img.shields.io/badge/Nmap-4682B4?style=for-the-badge&logo=nmap&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

<!-- Methodologies & Technical Focus -->
![IP Address Recon](https://img.shields.io/badge/IP_Address_Recon-2E8B57?style=for-the-badge&logo=wireshark&logoColor=white)
![Password Recovery](https://img.shields.io/badge/Password_Recovery-D14836?style=for-the-badge&logo=1password&logoColor=white)
![Data Extraction](https://img.shields.io/badge/Data_Extraction-8E44AD?style=for-the-badge&logo=elasticsearch&logoColor=white)

<!-- Target & Lab Info -->
![Target: Mediroza General Hospital](https://img.shields.io/badge/Target-Mediroza_General_Hospital-E63946?style=for-the-badge&logo=hospital&logoColor=white)
![Network Walks](https://img.shields.io/badge/Network_Walks-008080?style=for-the-badge&logo=cisco&logoColor=white)

Full black-box penetration test. Identify vulnerabilities, exploit them to demonstrate real impact, and document all findings in a
professional report.

---

## 🔎 Project Overview

This project executes a structured Penetration Testing and Vulnerability Assessment to evaluate and secure a target environment. The primary objective is to identify system vulnerabilities, demonstrate exploit vectors, and deliver actionable remediation strategies.

The assessment is structured into four sequential milestones:

* Initial Access: Reconnaissance, target scanning, and securing an initial entry point.
  
* Data Extraction: Navigating file systems and retrieving sensitive internal assets.
  
* Attack & Credential Cracking: Simulating system exploitation and cracking targeted passwords.

* PenTest Report: Documenting security flaws, technical findings, and mitigation recommendations

---

## 🎯 Objectives

#### Milestone 1: Target Reconnaissance & Initial Access
* Objective: Conduct initial security assessments to identify unlinked endpoints, exposed directories, and input vulnerabilities across the web application environment.

* Key Tasks:

Perform target footprinting and directory enumeration using tools like Nmap and Gobuster.

Analyze authentication mechanisms and input handling controls.

Identify configuration issues to simulate gaining unauthorized access to restricted application areas.

---

#### Milestone 2: File Analysis & Credential Recovery
* Objective: Analyze restricted assets and retrieve protected data through local file decryption and password recovery techniques.

* Key Tasks:

Identify encryption schemes applied to retrieved documents.

Select appropriate security utilities and wordlists (e.g., John the Ripper, Hashcat) for password recovery.

Evaluate multiple decryption strategies based on file structures and hashes.

---

#### Milestone 3: Data Analysis & Risk Identification
* Objective: Examine retrieved assets and file metadata to locate underlying data exposures within the client infrastructure.

* Key Tasks:

Inspect file properties, hidden metadata, and embedded content across extracted files.

Identify secondary server exposures, exposed employee salary lists, and hospital shareholder documentation.

Document data exposure findings for risk assessment.

---

#### Milestone 4: Penetration Testing Report Documentation
* Objective: Compile technical findings into a professional security audit report detailing vulnerabilities, impact ratings, and remediation steps.

* Report Structure:

Executive Summary: High-level summary of engagement objectives, critical findings, and business risk profile.

Scope & Methodology: Target definitions, tools used (Kali Linux, VirtualBox, Nmap), and assessment boundaries.

Findings & Proof of Concept: Step-by-step evidence and technical proof of exploitation for each milestone.

Risk Rating: Vulnerability classification based on industry severity standards (Critical, High, Medium, Low).

Recommendations & Remediation: Actionable defense-in-depth guidance to patch identified weaknesses and harden the system.

---

## M1

## M i l e s t o n e 1

Attack the website and find the 3 confidential PDF lab reports of patients.

<img width="398" height="224" alt="Screenshot 2026-09-28 213214" src="https://github.com/user-attachments/assets/f33a4790-bedb-49ce-91b5-693f0871b0d5" />

---
* Reconnaissance and Initial Accesss.

  Enumerate the external attack surface, identify accessible application components, and access authentication mechanisms. 

<img width="639" height="332" alt="Screenshot 2026-09-27 210748" src="https://github.com/user-attachments/assets/12bff445-64d1-4d02-975c-ca35c0008a39" />

---
* Tools include:

Nmap – A powerful network scanning and discovery tool used to detect live hosts, open ports, running services, and operating systems on a network.

Gobuster – A high-speed command-line tool used to brute-force and discover hidden directories, files, and DNS subdomains on web servers.

Nikto – An open-source web server scanner that tests for dangerous files, outdated server software, configuration vulnerabilities, and security risks.

WhatWeb – A web technology identifier that scans websites to detect technologies in use, including CMS platforms, web servers, embedded scripts, and analytics tools.
---
* Outputs:

<img width="632" height="338" alt="Screenshot 2026-09-28 215455" src="https://github.com/user-attachments/assets/e5689dfb-f3db-4f91-be56-87535722162f" />

Proof of access and the 3 retrieved PDF files.

---
## M2

## M i l e s t o n e 2

* Crack the encryption on all 3 retrieved files.

<img width="398" height="227" alt="Screenshot 2026-09-28 215649" src="https://github.com/user-attachments/assets/10173d70-c268-4c97-88f5-6cd81ba4fe8d" />

Recover the passwords of those locked pdfs that we get from patient portal.

---
* Tools include:

Python – A versatile, high-level programming language widely used in cybersecurity for automating security workflows, writing custom analysis scripts, and handling file data programmatically.

pikepdf – A Python library based on QPDF designed for inspecting, manipulating, and modifying the structure and encryption properties of PDF files.

John the Ripper – A fast, open-source password security auditing tool designed to test password strength and audit password hashes across various formats and operating systems.

Networkwalks tools – A suite of training utilities and scripts provided within the Networkwalks curriculum for performing controlled lab exercises, credential auditing, and security lab demonstrations.

PDF Password Recovery – A general classification of utilities or software designed to analyze PDF document protection settings, remove known restrictions, or test password strength on encrypted PDF documents.
---
* Outputs:

<img width="398" height="313" alt="red1" src="https://github.com/user-attachments/assets/0c5f40e7-8673-40ac-a033-e44f7f31cf55" />

<img width="399" height="310" alt="red2" src="https://github.com/user-attachments/assets/5a7e3285-1933-41ad-a9ce-58dd286dba7a" />

<img width="397" height="317" alt="red3" src="https://github.com/user-attachments/assets/8f435b8a-eb37-4b9d-8b8b-bebb20e86e0f" />

Recovered contents of all 3 files with proof of successful access.

---
## M3

## M i l e s t o n e 3

* Find the critical data exposure on the client server.

<img width="400" height="227" alt="Screenshot 2026-09-28 220926" src="https://github.com/user-attachments/assets/e9db61cf-e5dc-4ce5-992f-7bac4744e014" />

• Find the salaries of all hospital employees.

• Find the shareholder details of the hospital.

---

* Tools include:
 Exiftool - Deep structural metadata extraction and recursive stream analysis on decrypted PDF files.

    ```bash
    exiftool -password '!@#$%^&' patient_report_3.pdf
     ```

    ```bash
    exiftool -password 'password' patient_report_2.pdf
    ```

    ```bash
    exiftool -password '123456' patient_report_1.pdf
    ```

Commands - 

Database Backup Discovery

Acting on the metadata comment, the following URL was accessed:

https://medirozahospital.com/old/

A publicly accessible database backup was found with no authentication required:

mediroza_db_backup_2019.sql — 7KB 

wget https://medirozahospital.com/old/mediroza_db_backup_2019.sql

Old Directory

```bash
curl -s -o mediroza_db_backup_2019.sql https://[TARGET_DOMAIN]/old/mediroza_db_backup_2019.sql
```
---

* Outputs:




















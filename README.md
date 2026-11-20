# NetworkWalks B084 Week3 | PDF Password Cracking

I recovered the passwords for two encrypted  PDFs and verified each result by opening the corresponding document and reading its flag. The first task used John the Ripper (JtR) on Kali Linux. The second used the Networkwalks browser-based tools.

| Project Module | Training document | Recovered password | Flag inside the document |
| --- | --- | --- | --- |
| W3-PM1 · John the Ripper | `My Locked PDF1.pdf` | `good-luck` | `nw{networkwalks_flag1_jtr_270521_1}` |
| W3-PM2 · Networkwalks Tools | `My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf` | `password1` | `nw{cybersecurity_flag_captured_2608}` |

## Task 1 · Recovering the password with John the Ripper

I used an online hash calculator to extract the PDF’s password-verification data and saved it as `my-locked-pdf1-hash.txt`. John the Ripper recovered the password on Kali Linux. The terminal screenshot shows a previously recovered result: JtR displays `good-luck` and reports one password hash cracked with zero remaining. I entered the password in the PDF viewer and confirmed that the document displayed the JtR flag.

**Online Hash Generated:**
<img width="1917" height="918" alt="online hash calcuator" src="https://github.com/user-attachments/assets/fd33f530-b08e-4e90-bcae-a46f9e1d2648" />

**Terminal Results:**
<img width="1915" height="922" alt="jrt password cracked" src="https://github.com/user-attachments/assets/e45ff890-9946-4f0f-b6ac-be2486c7c70d" />

**PDF Password Prompt:**
<img width="746" height="650" alt="password unlocked file" src="https://github.com/user-attachments/assets/27db5c49-b3ce-4c47-aec9-b682cd9a16a7" />

**File Unlocked:**
<img width="1055" height="1491" alt="cracked-my-locked-pdf1" src="https://github.com/user-attachments/assets/e0d64df9-c9fa-467c-b3b2-95b2cdb2bbb2" />

---


## Task 2 · Recovering the password with Networkwalks

I used the PDF mode of the Networkwalks Hash Calculator on the WK3-PM2 document. The calculator identified the PDF as encrypted and extracted its password-verification data. The Networkwalks Password Cracker reported a match for `password1` after trying 91 of 100 common passwords. I verified the result by entering the password in the viewer and opening the page containing the second flag.

**Hash Generated:**
<img width="1916" height="886" alt="nw-hash-solved" src="https://github.com/user-attachments/assets/c744df6f-8eac-430f-b8db-7e29a65c2f91" />

**Password Identified:**
<img width="1916" height="875" alt="nw-password-revealed" src="https://github.com/user-attachments/assets/1c322f32-93d8-4fe8-8c4d-dda293f6f395" />

**Password Prompt:**
<img width="1912" height="890" alt="nw-unlocked-file" src="https://github.com/user-attachments/assets/c23adbbf-48af-4274-b4ca-5ca0ac90b94d" />

**File Unlocked:**
<img width="567" height="737" alt="nw-unlocked-pdf" src="https://github.com/user-attachments/assets/d9142f87-4cee-482e-90c8-f4a900008618" />

---

## What the lab demonstrated

The WK3-PM2 PDF used a 128-bit encryption key, yet its password appeared in a list of just 100 common passwords. The tool found a password that the document accepted by testing likely guesses. For sensitive PDFs, a long, unique, randomly generated password makes that approach less effective.

---

## Author

**Garcia Forrest**

Cybersecurity Student (CC) B084

LinkedIn: www.linkedin.com/in/garcia-forrest


---
title: "lames - HTB Write-up"
date: 2026-03-11
tags:
  - htb
  - writeup
---

# 🎯 lames - Hack The Box

**Difficulty:** [Easy / Medium / Hard / Insane]  
**OS:** [Linux / Windows]  
**IP Address:** [10.10.11.x]  

---

## 🔍 1. Reconnaissance & Enumeration

### Nmap Scan
*Initial port scan to identify running services.*

```bash
nmap -sC -sV -p- [IP] 
```

### Web Discovery
*Finding hidden directories and files.*

```bash
gobuster dir -u http://[IP] -w /usr/share/wordlists/dirb/common.txt
```

---

## 🛡️ 2. Exploitation
### The Vulnerability
*Explain what was found (e.g., Weak Credentials, RCE, SQLi).*

### Getting the Flag
*The exact commands run to navigate the system or database to retrieve the final flag.*

```bash
cat user.txt
```

---

## 🔝 3. Privilege Escalation
### Enumeration
*Searching for a path to Root/Administrator.*

### Root Flag
*Final steps to compromise the machine.*

---

## 📝 4. Final Thoughts
**Key Takeaways:**
* [What did you learn from this machine?]
* [Which tools were most effective?]

---
*Note: This write-up is for educational purposes and personal tracking only.*
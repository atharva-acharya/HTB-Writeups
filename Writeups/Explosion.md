---
title: Explosion - HTB Write-up
date: 2026-03-11
tags:
  - htb
  - writeup
  - windows
---

# 🎯 Explosion - Hack The Box

**Difficulty:** Very Easy  
**OS:** Windows  

---

## 📋 Tasks

### Task 1
**Question:** What does the 3-letter acronym RDP stand for?
**Answer:** Remote Desktop Protocol
**How I found it:** Google

### Task 2
**Question:** What is a 3-letter acronym that refers to interaction with the host through a command line interface?
**Answer:** CLI
**How I found it:** 

### Task 3
**Question:** What about graphical user interface interactions?
**Answer:** GUI
**How I found it:** 

### Task 4
**Question:** What is the name of an old remote access tool that came without encryption by default and listens on TCP port 23?
**Answer:** Telnet
**How I found it:** 

### Task 5
**Question:** What is the name of the service running on port 3389 TCP?
**Answer:** ms-wbt-server
**How I found it:** `nmap -sV -p3389 10.129.4.46`
![](assets/Pasted%20image%2020260311190327.png)

### Task 6
**Question:** What is the switch used to specify the target host's IP address when using xfreerdp?
**Answer:** `/v:`
**How I found it:** 

### Task 7
**Question:** What username successfully returns a desktop projection to us with a blank password?
**Answer:** Administrator
**How I found it:** 



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
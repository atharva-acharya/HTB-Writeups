---
title: "[Machine Name] - HTB Write-up"
date: YYYY-MM-DD
tags:
---
# 🎯 [Machine Name] - Hack The Box

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

**Open Ports:**
* **Port 22:** SSH
* **Port 80:** HTTP (Web Server)
* *(Add others as needed)*

### Web Enumeration
*Notes on directory busting, subdomains, or interesting web elements.*

```bash
# Gobuster, Feroxbuster, or Ffuf commands go here
```
* **Findings:** [Note any interesting directories or files found]

---

## 🚪 2. Initial Access (Foothold)

### Vulnerability Discovery
*Describe how you found the vulnerability. What was the exact weakness?*

### Exploitation
*Explain the steps you took to exploit the vulnerability.*

```bash
# Exploit commands or reverse shell payload go here
```

> **User Flag:** > `[Paste user.txt hash here]`

---

## 👑 3. Privilege Escalation

### Local Enumeration
*What did you find after getting your initial shell? (e.g., LinPEAS results, SUIDs, cron jobs).*

### The Vulnerability (Path to Root)
*Explain the misconfiguration that allows you to escalate your privileges.*

### Exploitation
*The exact commands run to become root.*

```bash
# Privilege escalation commands go here
```

> **Root Flag:** > `[Paste root.txt hash here]`

---

## 💡 4. Conclusion & Lessons Learned

* **What I learned:** [Brief note on a new technique, tool, or concept you picked up]
* **Rabbit Holes:** [Did you get stuck anywhere? Note it here so you remember for next time]
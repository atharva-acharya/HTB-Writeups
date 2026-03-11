---
title: "[Machine Name] - HTB Starting Point"
date: YYYY-MM-DD
tags:
  - htb
  - writeup
  - starting-point
  - linux # or windows
  - very-easy # or easy
---
# 🎯 [Machine Name] - HTB Starting Point

**Difficulty:** [Very Easy / Easy]  
**OS:** [Linux / Windows]  
**IP Address:** [10.129.x.x]  

---

## 📝 1. Guided Tasks & Questions

*Log the questions asked by the HTB platform and how you found the answers.*

**Task 1: Which TCP port is open on the machine?**
**Answer:** [e.g., 6379]
**How I found it:**
```bash
nmap -sV -p- [IP]
```

**Task 2: Which service is running on the port that is open on the machine?**
**Answer:** [e.g., Redis]
**How I found it:** Nmap service scan output.

**Task 3: [Paste the next question here]**
**Answer:** [Your answer]
**How I found it:** [Brief explanation or command]

---

## 🔍 2. Reconnaissance & Enumeration

### Nmap Scan Details
*Full output and notes from the initial port scan.*

```bash
# Paste your full Nmap command and interesting output here
```

### Service Enumeration
*Notes on interacting with the specific service (e.g., Redis, SMB, FTP).*

```bash
# Commands used to connect to the service (e.g., redis-cli -h [IP])
```

---

## 🚪 3. Exploitation & The Flag

### The Vulnerability
*Explain the misconfiguration that allowed access (e.g., Redis server left open with no authentication).*

### Getting the Flag
*The exact commands run to navigate the system or database to retrieve the final flag.*

```bash
# Paste your commands here (e.g., keys *, get flag)
```

> **Root/Final Flag:** > `[Paste the flag hash here]`

---

## 💡 4. Conclusion & Lessons Learned

**What I learned:** [Brief note on the protocol or tool you learned, like how to use redis-cli]

**Commands to remember:** `[command 1]` - [What it does]
`[command 2]` - [What it does]
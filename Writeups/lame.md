---
title: Untitled - HTB Write-up
date: 2026-03-11
tags:
  - htb
  - writeup
---

# 🎯 Untitled - Hack The Box

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
---
title: Reedemer - HTB Starting Point
date: 2026-03-11
tags:
  - htb
  - writeup
  - starting-point
  - linux
  - very-easy
---
# 🎯 Reedemer - HTB Starting Point

**Difficulty:** Very Easy
**OS:** Linux  

---

## 📝 1. Guided Tasks & Questions

Task 1: Which TCP port is open on the machine?
Answer: 6379
How I found it:
```bash
nmap -sV -p- [IP]
```

![[Pasted image 20260311171617.png]]

Task 2: Which service is running on the port that is open on the machine?
Answer: Redis

Task 3: What type of database is Redis? Choose from the following options: (i) In-memory Database, (ii) Traditional Database
Answer: In-memory Database

Task 4:Which command-line utility is used to interact with the Redis server? Enter the program name you would enter into the terminal without any arguments.
Answer: redis-cli
How I found it: simple google search

Task 5: Which flag is used with the Redis command-line utility to specify the hostname?
Answer: `-h`
How I found it: `redis-cli --help`

Task 7:Once connected to a Redis server, which command is used to obtain the information and statistics about the Redis server?
Answer: info
How I found it: `redis-cli --cluster help` 

![[Pasted image 20260311172944.png]]

Task 8: What is the version of the Redis server being used on the target machine?
Answer: `5.0.7`
How I found it: 
![[Pasted image 20260311173059.png]]

Task 9: Which command is used to select the desired database in Redis?
Answer: select
How I found it: google 

Task 9: How many keys are present inside the database with index 0?
Answer: 4
How I found it:
![[Pasted image 20260311173341.png]]

Task 10: Which command is used to obtain all the keys in a database?
Answer: `KEYS *`
How I found it: Google

---

## 🚪 2. Exploitation & The Flag

### The Vulnerability
Redis server left open with no auth
### Getting the Flag
*The exact commands run to navigate the system or database to retrieve the final flag.*

```bash
redis-cli -h [IP]
```

```bash
info
```

```bash
salect 0
```

```bash
KEYS *
```

```bash
GET KEY
```

> **Root/Final Flag:** > `[Paste the flag hash here]`

---

## 💡 4. Conclusion & Lessons Learned

**What I learned:** [Brief note on the protocol or tool you learned, like how to use redis-cli]

**Commands to remember:** `[command 1]` - [What it does]
`[command 2]` - [What it does]
# Week 3 — Password Cracking with NetworkWalks Tools

## Overview

This repository documents **Week 3** of the Cybersecurity Internship. It records a password-cracking laboratory exercise performed with NetworkWalks tools, including the supplied PDF hash and screenshots collected during the session.

The exercise was conducted for authorized cybersecurity training. Password-cracking techniques must only be used against systems and data for which explicit permission has been granted.

---

## Lab Evidence

The screenshots below are arranged in chronological order according to the time shown in each filename.

### 1. Environment Setup — 19:19:20

![NetworkWalks password-cracking environment at 19:19:20](Screenshot%202026-11-19%20191920.png)

**Figure 1:** Initial laboratory environment and tool setup used for the Week 3 password-cracking exercise.

### 2. Hash Preparation — 19:23:18

![Hash preparation stage at 19:23:18](Screenshot%202026-11-19%20192318.png)

**Figure 2:** Preparation and loading of the supplied password hash beginning at 19:23:18.

### 3. Cracking Workspace — 19:27:50

![Cracking workspace at 19:27:50](Screenshot%202026-11-19%20192750.png)

**Figure 3:** NetworkWalks cracking workspace and exercise configuration displayed at 19:27:50.

### 4. Attack Configuration — 19:29:09

![Password attack configuration at 19:29:09](Screenshot%202026-11-19%20192909.png)

**Figure 4:** Configuration of the password-testing activity and attack parameters at 19:29:09.

### 5. Cracking Activity — 19:30:10

![Password-cracking activity at 19:30:10](Screenshot%202026-11-19%20193010.png)

**Figure 5:** Active password-cracking process, progress information, or command execution captured at 19:30:10.

### 6. Continued Analysis — 19:41:57

![Continued cracking analysis at 19:41:57](Screenshot%202026-11-19%20194157.png)

**Figure 6:** Continued analysis or tool output captured during the laboratory exercise at 19:41:57.

### 7. Result Review — 19:43:12

![Result review at 19:43:12](Screenshot%202026-11-19%20194312.png)

**Figure 7:** Review of cracking progress or available result information at 19:43:12.

### 8. Verification Stage — 19:44:07

![Verification stage at 19:44:07](Screenshot%202026-11-19%20194407.png)

**Figure 8:** Verification or follow-up test performed during the 19:44:07 stage of the exercise.

### 9. Tool Output — 19:44:22

![Password-cracking tool output at 19:44:22](Screenshot%202026-11-19%20194422.png)

**Figure 9:** NetworkWalks tool output or status information captured at 19:44:22.

### 10. Progress and Findings — 19:44:49

![Progress and findings at 19:44:49](Screenshot%202026-11-19%20194449.png)

**Figure 10:** Evidence showing the lab progress and testing findings at 19:44:49.

### 11. Final Evidence — 19:45:33

![Final laboratory evidence at 19:45:33](Screenshot%202026-11-19%20194533.png)

**Figure 11:** Final screen or result evidence captured at 19:45:33, completing the documented laboratory sequence.

---

## Repository Files

| File | Description |
|---|---|
| [`HASH 1.txt`](HASH%201.txt) | Supplied PDF password hash used in the lab |
| [`Screenshot 2026-11-19 191920.png`](Screenshot%202026-11-19%20191920.png) | Laboratory setup evidence |
| [`Screenshot 2026-11-19 192318.png`](Screenshot%202026-11-19%20192318.png) | Hash preparation evidence |
| [`Screenshot 2026-11-19 192750.png`](Screenshot%202026-11-19%20192750.png) | Cracking workspace evidence |
| [`Screenshot 2026-11-19 192909.png`](Screenshot%202026-11-19%20192909.png) | Attack configuration evidence |
| [`Screenshot 2026-11-19 193010.png`](Screenshot%202026-11-19%20193010.png) | Active cracking evidence |
| [`Screenshot 2026-11-19 194157.png`](Screenshot%202026-11-19%20194157.png) | Continued analysis evidence |
| [`Screenshot 2026-11-19 194312.png`](Screenshot%202026-11-19%20194312.png) | Result review evidence |
| [`Screenshot 2026-11-19 194407.png`](Screenshot%202026-11-19%20194407.png) | Verification evidence |
| [`Screenshot 2026-11-19 194422.png`](Screenshot%202026-11-19%20194422.png) | Tool output evidence |
| [`Screenshot 2026-11-19 194449.png`](Screenshot%202026-11-19%20194449.png) | Progress and findings evidence |
| [`Screenshot 2026-11-19 194533.png`](Screenshot%202026-11-19%20194533.png) | Final laboratory evidence |

---

## Hash Information

[`HASH 1.txt`](HASH%201.txt) contains a PDF password hash beginning with `$pdf$`. This format identifies the sample as a PDF hash suitable for testing by a compatible password-cracking tool.

> The hash is retained only as authorized laboratory evidence. Do not reuse or attempt to crack real credentials outside an approved test scope.

---

## Lab Objectives

1. Understand the difference between passwords and password hashes.
2. Identify the supplied PDF hash format.
3. Demonstrate password-testing techniques in an authorized environment.
4. Record the commands, tool output, and relevant screenshots.
5. Explain defensive measures that reduce password attack risk.

---

## Example Commands

These commands are for authorized laboratory use only.

### John the Ripper

```bash
john --wordlist=/path/to/wordlist.txt "HASH 1.txt"
```

### Hashcat

```bash
# Verify the PDF mode supported by the installed Hashcat version
hashcat -m 10500 -a 0 "HASH 1.txt" /path/to/wordlist.txt
```

---

## Findings Template

Add verified lab results after confirming them from the screenshots:

- **Hash type:** PDF password hash
- **Source file:** `HASH 1.txt`
- **Tool used:** _Add tool name and version_
- **Attack method:** _Dictionary / rules / mask / brute-force_
- **Wordlist:** _Document the approved wordlist used_
- **Result:** _Success / no match found_
- **Recovered password:** _Keep private or redact publicly_
- **Duration:** _Add elapsed time_

---

## Security Recommendations

- Use strong, unique passwords or passphrases.
- Prefer long passwords or passphrases over predictable words.
- Enable multifactor authentication wherever available.
- Use account lockouts or throttling to slow repeated attempts.
- Use modern, salted password-hashing algorithms.
- Monitor authentication logs for spraying and brute-force patterns.
- Educate users against password reuse and phishing.
- Restrict access to password hashes and sensitive documents.

---

## Ethical and Legal Notice

Password testing must only be performed on systems, files, or accounts that the tester owns or is explicitly authorized to assess. The evidence in this repository is for defensive cybersecurity training and awareness.

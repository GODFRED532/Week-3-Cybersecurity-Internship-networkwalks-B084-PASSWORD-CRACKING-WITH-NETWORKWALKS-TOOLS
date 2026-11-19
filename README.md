# Week 3 — Password Cracking with NetworkWalks Tools

## Overview

This repository contains the evidence for **Week 3** of the Cybersecurity Internship, covering password-cracking concepts and practical exercises using NetworkWalks tools.

The lab is based on an authorized, controlled exercise performed for learning purposes. Hashes and credentials must only be handled in environments and circumstances where testing is explicitly permitted.

## Repository Contents

| File | Purpose |
|---|---|
| [`HASH 1.txt`](HASH%201.txt) | PDF hash sample used for the cracking exercise |
| [`Screenshot 2026-11-19 191920.png`](Screenshot%202026-11-19%20191920.png) | Lab evidence — 19:19:20 |
| [`Screenshot 2026-11-19 192318.png`](Screenshot%202026-11-19%20192318.png) | Lab evidence — 19:23:18 |
| [`Screenshot 2026-11-19 192750.png`](Screenshot%202026-11-19%20192750.png) | Lab evidence — 19:27:50 |
| [`Screenshot 2026-11-19 192909.png`](Screenshot%202026-11-19%20192909.png) | Lab evidence — 19:29:09 |
| [`Screenshot 2026-11-19 193010.png`](Screenshot%202026-11-19%20193010.png) | Lab evidence — 19:30:10 |
| [`Screenshot 2026-11-19 194157.png`](Screenshot%202026-11-19%20194157.png) | Lab evidence — 19:41:57 |
| [`Screenshot 2026-11-19 194312.png`](Screenshot%202026-11-19%20194312.png) | Lab evidence — 19:43:12 |
| [`Screenshot 2026-11-19 194407.png`](Screenshot%202026-11-19%20194407.png) | Lab evidence — 19:44:07 |
| [`Screenshot 2026-11-19 194422.png`](Screenshot%202026-11-19%20194422.png) | Lab evidence — 19:44:22 |
| [`Screenshot 2026-11-19 194449.png`](Screenshot%202026-11-19%20194449.png) | Lab evidence — 19:44:49 |
| [`Screenshot 2026-11-19 194533.png`](Screenshot%202026-11-19%20194533.png) | Lab evidence — 19:45:33 |

## Exercise Objectives

1. Understand the difference between passwords and password hashes.
2. Identify the PDF hash format supplied for the exercise.
3. Demonstrate dictionary and/or brute-force password-testing techniques in an authorized environment.
4. Record commands, results, and relevant evidence.
5. Explain defensive measures that reduce password attack risk.

## Hash Information

The supplied hash in [`HASH 1.txt`](HASH%201.txt) is in PDF hash format. It begins with `$pdf$`, which identifies it as a hash suitable for a PDF-password cracking tool.

> The hash is preserved as laboratory evidence. Do not reuse, publish, or attempt to crack real-world credentials outside an approved assessment scope.

## Lab Steps

### 1. Prepare the environment

- Use an isolated virtual machine or authorized laboratory system.
- Confirm the password-cracking tool is installed and compatible with PDF hashes.
- Keep the hash file and screenshots in the repository evidence folder.

### 2. Prepare a wordlist

A cracking exercise commonly uses a local wordlist:

```bash
# Example only: run against an authorized lab hash
# Replace HASH-1.txt with the repository's file name
john --wordlist=/path/to/wordlist.txt "HASH 1.txt"
```

Hashcat can use the PDF hash format when its PDF mode is available:

```bash
# Example syntax; verify the supported PDF mode on the installed tool version
hashcat -m 10500 -a 0 "HASH 1.txt" /path/to/wordlist.txt
```

### 3. Run the test

- Start with a small, relevant dictionary.
- Apply mangling rules if permitted by the lab instructions.
- Record the tool version, hash mode, attack mode, and elapsed time.
- Take screenshots of the command and successful result, or of a completed attempt when no match is found.

### 4. Verify and document

- Verify any recovered password using the lab target or PDF itself.
- Do not display real credentials in public documentation.
- Add the command, result, tool version, and timestamp to this report.

## Findings

Add the final verified results here after completing the lab:

- **Hash type:** PDF password hash
- **Source file:** `HASH 1.txt`
- **Tool used:** _Add tool name and version_
- **Attack method:** _Dictionary / rules / mask / brute-force_
- **Wordlist:** _Document the approved wordlist used_
- **Result:** _Success / no match found_
- **Recovered password:** _Store separately or redact in public documentation_
- **Duration:** _Add elapsed time_

## Security Recommendations

- Use strong, unique passwords with at least 12–16 characters when practical.
- Prefer passphrases over predictable words or common patterns.
- Enable multifactor authentication wherever available.
- Lock accounts or slow repeated attempts with appropriate controls.
- Use salted, modern password hashing algorithms instead of legacy formats.
- Educate users about phishing and credential reuse.
- Monitor authentication logs for password spraying and brute-force patterns.
- Restrict the distribution of password hashes and encrypted documents.

## Evidence

### Tool setup and environment

![Lab evidence 191920](Screenshot%202026-11-19%20191920.png)

### Hash preparation and cracking activity

![Lab evidence 192318](Screenshot%202026-11-19%20192318.png)

![Lab evidence 192750](Screenshot%202026-11-19%20192750.png)

![Lab evidence 192909](Screenshot%202026-11-19%20192909.png)

![Lab evidence 193010](Screenshot%202026-11-19%20193010.png)

### Results and verification

![Lab evidence 194157](Screenshot%202026-11-19%20194157.png)

![Lab evidence 194312](Screenshot%202026-11-19%20194312.png)

![Lab evidence 194407](Screenshot%202026-11-19%20194407.png)

![Lab evidence 194422](Screenshot%202026-11-19%20194422.png)

![Lab evidence 194449](Screenshot%202026-11-19%20194449.png)

![Lab evidence 194533](Screenshot%202026-11-19%20194533.png)

## Ethical and Legal Notice

Password testing should only be performed on systems, files, or accounts that the tester owns or is explicitly authorized to assess. The techniques demonstrated in this repository are for defensive cybersecurity training and awareness.

# Cyber Security Journey

This repo is a learning log, not a portfolio.  
Hence it tracks what I've actually studied, built, and understood.
It will contain links to the projects that i have built, and writeups for the paths in TryHackMe that i do.
It will also contain the writeups regarding CTF's and BugBounty (if i ever get into that)

P.S. (this readme file gets updated whenever i do something new)
---

## What I've learned so far

### TryHackMe — Pre-Security Path
*Completed May 2026 · 19h 10m · [writeup →](./tryhackme-writeups/pre-security/)*

Networking, web protocols, OS fundamentals, CLI, data encoding, SQL basics, cryptography, and a first taste of offensive tooling. Two things that actually stuck:

- The **key distribution problem** — I kept thinking "if both sides need the same key, how do you share it securely in the first place?" Then asymmetric cryptography was introduced and it solved exactly that. That clicked hard.
- **Gobuster** — first time watching it throw hundreds of directory names at a target automatically. That's when offensive security stopped feeling abstract.

---

### RCPT — Ransomware Crypto Payment Tracker
*March 2026 · [repo →](https://github.com/Krish-Anand-dev/RCPT)*

Built a blockchain forensics dashboard to trace ransomware payments on Ethereum.

**What I learned about:**
- How ransomware attackers actually move money, splitting funds across wallets, chaining rapid hops, using round amounts to blend in. These aren't random; they're deliberate obfuscation patterns.
- Blockchain transparency as a forensics tool. Everything is public, timestamped, and traceable BUT the challenge is interpretation, not access.
- How to build a detection engine: five pattern modules running in parallel (splitting, chaining, large transfers, velocity, round amounts), each contributing weighted points to a 0–100 risk score per wallet.
- Why enterprise tools like Chainalysis exist and what makes this problem hard at scale.

---

### GoReSym — Binary Triage Toolkit
*March 2026 · [repo →](https://github.com/Krish-Anand-dev/go-binary-triage)*

Built a CLI companion to GoReSym (Mandiant's Go binary symbol recovery tool) that takes its JSON output and produces a structured analyst report, risk score, inferred capabilities, IOCs, suspicious strings.

**What I learned about:**
- How Go binaries differ from C/C++ — they retain a lot of metadata even when "stripped", which is why GoReSym can recover symbols
- What malware analysts actually look for in a binary: network comms, crypto operations, command execution, persistence mechanisms
- Behavioural function classification — grouping recovered function names into capability buckets to infer what a binary is doing without running it
- The existing tooling ecosystem: IDA, Ghidra, Binary Ninja — and where GoReSym fits as a pre-processing step

---

## What's next

- **TryHackMe SOC Level 1** — Wireshark, SIEM, Splunk, phishing analysis
---

## Platforms

- [TryHackMe](https://tryhackme.com/p/krishanand.dev)
- [GitHub](https://github.com/Krish-Anand-dev)
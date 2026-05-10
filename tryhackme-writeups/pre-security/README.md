# TryHackMe — Pre-Security Path

**Completed:** 10 May 2026 · **Duration:** 19h 10m · **Cert:** THM-GNAONIICFH

---

## How I actually did this

Not in order. I started with networking and web (DNS, HTTP, how the internet works), then hit a wall with pure theory and jumped ahead to OS and software — Linux CLI, Windows, data representation, SQL basics. Went back and filled in computer fundamentals (cloud, virtualisation, client-server) at the end.

Turns out that was fine. The modules are self-contained enough that the order didn't matter much.

---

## What's covered

| Module | Topics |
|--------|--------|
| Intro | Offensive vs defensive security, careers in cyber |
| Networking | OSI model, LAN, packets & frames, NAT |
| Web | DNS, HTTP, how websites work end-to-end |
| Computer Fundamentals | Hardware basics, virtualisation, cloud models |
| Operating Systems | Windows + Linux CLI, OS security controls |
| Software Basics | Binary/hex, encoding, Python/JS logic, SQL |
| Attacks & Defenses | CIA triad, cryptography, gobuster, hydra |

---

## Two things that actually stuck

**Cryptography — the key distribution problem**

When I was going through symmetric encryption, I kept thinking: *if both sides need the same key, how do you share it securely in the first place?* That felt like a fundamental contradiction. Then the next section introduced asymmetric cryptography — public/private keys — and it clicked immediately. The problem I was stuck on was exactly why asymmetric crypto was invented. That felt satisfying.

**Gobuster**

First time running `gobuster dir` and watching it automatically throw hundreds of directory names at a target — that was the moment offensive security stopped feeling abstract. You're not manually guessing. You're automating the brute work. That shift in thinking stuck with me.

---

## What's next

SOC Level 1 — Wireshark, SIEM, Splunk, phishing analysis.
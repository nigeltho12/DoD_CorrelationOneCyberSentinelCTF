# 🛡️ Cyber Sentinel CTF – June 2025 Write-up

**Username:** Eyeam_Legin  
**Total Score:** 975 points  
**Overall Rank:** 738th out of ~6,000 participants  
**Date:** June 14, 2025  
**Organizer:** Correlation One, sponsored by the U.S. Department of Defense  

---

## 🧭 Event Overview

The **Cyber Sentinel CTF** was a one-day, high‑stakes cybersecurity competition aimed at emerging and seasoned professionals. Key details:

- 👥 **Participants:** ~6,000 from universities, government agencies, private sector teams
- 🎯 **Rank Tiers:** Top 100 earn medals; top 1,000 receive official placement badges
- 🏆 **Prizes:** Awarded for overall ranking, challenge category leaders, and newcomer recognition
- 🎓 **Eligibility:** Open to all; multiple tracks included for students, professionals, and veterans
- 📚 **Support Role:** As an **Ambassador**, I helped recruit and mentor participants, organized community practice sessions, and provided day‑of support.

---

## ✅ Completed Challenges

| Name                        | Category                  | Points | Summary                                                                 |
|-----------------------------|---------------------------|--------|-------------------------------------------------------------------------|
| **Cafe Confidential**       | OSINT                     | 75     | Used image metadata to identify café locations via reverse search.      |
| **Problems in North TORbia**| OSINT                     | 150    | Analyzed PDF trails to expose operational details and retrieve a flag.  |
| **Secret.txt Society**      | Web Security              | 75     | Flag hidden behind disallowed `robots.txt` path.                        |
| **Field Reports Mayhem**    | Web Security              | 150    | Exploited parameter `id=1337` to access admin-level field reports.      |
| **Hidden in Plain Sight**   | Forensics                 | 75     | Extracted embedded flag using `steghide` with a discovered passphrase. |
| **Behind the Beat**         | Forensics                 | 75     | Converted audio file to spectrogram and spotted the hidden flag.        |
| **Encoded Evidence**        | Malware/Reverse Engineering | 75   | Decoded VBScript payload from Pastebin to reveal Base64 flag.          |
| **Hardcoded Lies**          | Malware/Reverse Engineering | 75   | Reverse engineered Python script; extracted flag string constant.       |
| **Packet Whisperer**        | Networking                | 75     | Analyzed PCAP capture; uncovered plaintext credentials for access.      |

---

## ❌ Unresolved Challenges

| Name               | Category     | Points | Summary & Roadblocks                                                         |
|--------------------|--------------|--------|-------------------------------------------------------------------------------|
| **ChatAPT**        | Networking   | 150    | Used `nc` to connect; AI responses were evasive/hallucinated, no valid flag. |
| **overSSHaring**   | Networking   | 200    | Retrieved disk images, attempted mounts and parsing; no usable SSH credentials. |
| **Hoasted Toasted**| Web/Recon    | 150    | Probed virtual hosts via Host header and SSL fuzzing; flag location remained hidden. |

---

## 🗂️ Repository Structure

CyberSentinelJune2025/
├── OSINT/
├── WebSecurity/
├── Forensics/
├── Networking/
├── Malware-ReverseEngineering/
├── Writeup/
│ └── CyberSentinel_Writeup.pdf
├── README.md


- Each category folder contains screenshots, scripts, extracted data.
- `Writeup/` includes comprehensive documentation and visual stats.

---

## 📈 Performance Analytics

- **Total Score:** 975 / 1,200 possible  
- **Challenge Solves:** 9 completed, 3 attempted  
- **Progress Visuals:** See `Writeup/ScoreboardStats/` for charts and timelines.

---

## 🧠 Lessons Learned

- **Leverage `robots.txt` & source comments** – They often reveal hidden but accessible paths.
- **Always extract all data** – Use tools like `strings`, `binwalk`, `steghide`, `sqlmap`, and `exiftool`.
- **Disk forensics takes time** – Mounting partitions requires `kpartx`, `fdisk`, or loop offset parsing.
- **Networking challenges demand patience** – Long delays or nonstandard ports (like 31337) are traps.
- **Look for redundancy** – Reused passwords or keys appeared across multiple services and files.
- **Document everything** – Clear notes and screenshots helped clarify approach, especially when stuck.
- **Pivot when stuck** – Switching challenges avoided time sinks and raised total score.

---

## 🎯 How to Contribute

Feel free to raise issues or pull requests if you have alternate solutions, corrections, or performance improvements. Thank you for exploring and happy hacking!

---

*— Eyeam_Legin, Cyber Sentinel Ambassador*  

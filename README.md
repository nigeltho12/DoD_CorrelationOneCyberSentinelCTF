# 🛡️ Cyber Sentinel CTF – June 2025 Write-up

**Username:** Eyeam_Legin  
**Total Score:** 975 points  
**Overall Rank:** 727th out of ~6,000 participants  
**Date:** June 14, 2025  
**Organizer:** Correlation One, sponsored by the U.S. Department of Defense  

---

## 🧭 Event Overview

The **Cyber Sentinel CTF** was a one-day, high‑stakes cybersecurity competition aimed at emerging and seasoned professionals. Key details:

- 👥 **Participants:** ~6,000 of cybersecurity enthusiasts from universities, government agencies, and private-sector teams
- 🏆 **Prizes:** Awarded for overall ranking
 
    🥇 1st Place: $5,000
  
    🥈 2nd Place: $2,500
  
    🥉 3rd Place: $1,000
  
    🎖️ 4th–10th Place: $500 each
  
    🎟️ Multiple $300 raffles distributed to active participants
  
    💰 Over $15,000 in total prizes awarded
  
- 🎓 **Eligibility:** U.S. citizens only, due to DoD sponsorship; targeted toward individuals interested in cybersecurity careers within or supporting the Department of Defense; multiple tracks included for students, professionals, and veterans
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



- Each category folder contains screenshots, scripts, extracted data.
- `Writeup/` includes comprehensive documentation and visual stats.

---

## 📈 Performance Analytics

- **Total Score:** 975  - 85th Percentile 
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

## 🤝 Let's Collaborate

If you're into CTFs, packet analysis, threat hunting, or just love breaking things to understand them — hit me up. I’m always down to team up, exchange ideas, or walk through challenges together.

---

*— Eyeam_Legin, Cyber Sentinel Ambassador*  

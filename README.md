# Reconnaissance & Scanning Lab

**Author:** Kalyan sai Ch  
**Environment:** Kali (attacker) + Metasploitable2 (target) — host-only / isolated network (authorized lab)

---

## Project overview
This repository contains a complete lab exercise for reconnaissance, port/service scanning and basic vulnerability assessment performed on an isolated Metasploitable2 virtual machine. All work is performed in a controlled host-only network and is strictly educational. I performed three Nmap scans to discover ports and services and one OpenVAS vulnerability scan. I recorded every step (terminal, scanner UI, and packet captures) and included the raw outputs, parsed summaries, evidence screenshots, PCAP(s) and a 5-minute demo video.

---

## Scans performed
- **Quick port discovery (SYN + top ports)**  
  **Purpose:** fast discovery of commonly used services.  
  **Example command used:**  

- **Full TCP sweep (SYN, all ports)**  
**Purpose:** comprehensive discovery of all TCP ports.  
**Example command used:**  

- **Full UDP sweep**  
**Purpose:** discover UDP services (slower, more noisy).  
**Example command used:**  

- **Service/version & OS detection**  
**Purpose:** identify service versions and attempt OS fingerprinting for vulnerability mapping.  
**Example command used:**  

- **OpenVAS vulnerability scan**  
**Purpose:** automated vulnerability detection and risk rating for discovered services.  
**Notes:** exported full HTML report and saved key findings (Critical/High/Medium) with remediation suggestions.

---

## Deliverables included
- Raw Nmap outputs and parsed summaries (/nmap-reports/)  
- OpenVAS full HTML report (/openvas-reports/)  
- Wireshark PCAP(s) and screenshots demonstrating traffic evidence (/wireshark-pcaps/)  
- iptables rules / mitigation proof (if applied) (/firewall/)  
- Demo video (5 minutes) showing the scan and findings (/demo/demo_video.mp4)  
- Evidence screenshots: nmap, OpenVAS, Wireshark, submission confirmation (/evidence/)  
- A concise findings & remediation summary (prioritized by severity)

---

## Notes & disclaimer
All tests were performed on lab machines I control (Metasploitable2) inside an isolated network. This repository is for educational purposes only — do not run these scans or DoS simulations against systems you do not own or have written permission to test.

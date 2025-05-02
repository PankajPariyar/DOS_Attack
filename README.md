# DoS Attack Using `hping3` (Manual SYN Flood)

⚠️ **DISCLAIMER:**  
This demonstration is for **educational and ethical testing only**. Never use this technique on systems you do not own or have permission to test. Misuse may lead to legal consequences.

## 📌 Description

This project showcases a basic **SYN Flood (DoS attack)** using the manual tool `hping3` on **Kali Linux**, targeting a vulnerable **Metasploitable2** machine. The attack floods the target with TCP SYN packets using a **spoofed IP address**. Wireshark is used to analyze the attack traffic.

## 🛠️ Tools Used

- Kali Linux (Attacker)
- hping3 (for SYN flood)
- Wireshark (for network analysis)
- Metasploitable2 (Target)

## 🚀 Attack Command

```bash
sudo hping3 -S --flood -a 10.10.10.10 -p 80 192.168.233.133 
---

## 🖼️ Wireshark Screenshot

This screenshot shows the SYN flood attack captured using Wireshark with the filter:

![Wireshark SYN Flood](Screenshots\dos_attack.png)


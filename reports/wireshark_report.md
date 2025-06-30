# Wireshark Network Traffic Analysis Report

## 🎯 Objective
Capture live network packets using Wireshark and identify basic protocols and traffic types.

---

## 🛠 Tools Used
- **Wireshark** (Packet analyzer)
- **Operating System**: [mention your OS, e.g., Windows 10 / Kali Linux]

---

## 📡 Traffic Generation Method
- Browsed a website (e.g., https://www.google.com)
- Used the command `ping google.com` to generate ICMP traffic

---

## 🧪 Protocol Filters & Observations

### 1. **TCP Traffic (`tcp`)**
- **Description**: TCP (Transmission Control Protocol) is a connection-oriented protocol used in most web-based applications.
- **Observation**:
  - Multiple TCP handshakes observed (`SYN`, `SYN-ACK`, `ACK`)
  - Active connections established with external servers (e.g., `google.com`)
  - Port 443 (HTTPS) and 80 (HTTP) were primarily used

📸 *[Include screenshot: tcp_traffic.png]*

---

### 2. **HTTP Traffic (`http`)**
- **Description**: HTTP (Hypertext Transfer Protocol) is used for unencrypted web communications.
- **Observation**:
  - Detected GET requests to websites
  - Header fields like `Host`, `User-Agent`, and `Accept` were visible
  - Server responded with `200 OK` or redirects (like `301 Moved Permanently`)

📸 *[Include screenshot: http_traffic.png]*

---

### 3. **DNS Traffic (`dns`)**
- **Description**: DNS (Domain Name System) resolves domain names to IP addresses.
- **Observation**:
  - DNS queries for domains like `google.com`, `youtube.com`
  - Response included IPv4 addresses (`A records`)
  - Communication over UDP port 53


---

## 📝 Summary of Findings
- Captured traffic successfully using Wireshark
- Identified and filtered three protocols: **TCP**, **HTTP**, and **DNS**
- Confirmed real-world behavior of browser and network tools
- Exported the `.pcap` file for future reference

---

## 📂 Deliverables
- `sample_capture.pcap` – The packet capture file
- `tcp.png`, `http.png`, `dns.png` – Filtered traffic screenshots
- `wireshark_report.md` – This analysis report

---

## ✅ Outcome
Hands-on understanding of live packet capture and analysis of different network protocols using Wireshark.

## 📋 Objective
Perform a network scan to identify open ports and running services on a local machine using **Nmap**.

---

## 🛠️ Tools Used
- **Nmap** – Network exploration and security auditing tool

---

## 🔧 Procedure
1. Installed **Nmap** on the system.
2. Performed a scan on the local machine using Nmap.
3. Identified open ports and running services.
4. Documented the scan results and analyzed the findings.

---

## 💻 Scan Command Used
```bash
nmap localhost
```

---

## 📡 Open Ports and Services

| Port | Service | Description |
|------|---------|-------------|
| 135 | MSRPC | Microsoft Remote Procedure Call service used for communication between Windows applications. |
| 445 | Microsoft-DS | SMB service used for file and printer sharing over the network. |

---

## 🔍 Findings
The scan identified **two open ports** on the local machine:
- **Port 135** → MSRPC
- **Port 445** → Microsoft-DS

These services are commonly used by Windows systems for inter-process communication and file/printer sharing over the network. While essential for normal Windows networking, these ports are also frequently targeted in attacks (e.g., SMB-based exploits), making it important to monitor and secure them.

---

## ✅ Result
Successfully scanned the local machine using Nmap and identified active ports and the services running on them.

---

## 📝 Conclusion
Nmap is a powerful network scanning tool used to discover hosts, identify open ports, and detect running services. This task provided practical, hands-on experience in **network reconnaissance** and **basic security assessment**, forming a foundation for more advanced vulnerability scanning tasks.

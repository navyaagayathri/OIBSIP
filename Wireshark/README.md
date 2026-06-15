## 📋 Objective
Capture and analyze live network traffic using **Wireshark** to understand how data is transmitted across a network, including the protocols involved and the information exchanged between source and destination devices.

---

## 🛠️ Tools Used
- **Wireshark** – Network protocol analyzer
- **Npcap** – Packet capture driver for Windows

---

## 🔧 Procedure
1. Installed **Wireshark** and **Npcap** on the system.
2. Selected the active **Wi-Fi** network interface for monitoring.
3. Started a live packet capture session.
4. Generated network traffic by browsing various websites.
5. Captured a sufficient number of packets successfully.
6. Analyzed the captured packets, examining source/destination addresses, protocols, and packet details.
7. Saved the capture file (`.pcapng`) for documentation and future reference.

---

## 📡 Observed Protocols

| Protocol | Description |
|----------|--------------|
| **TCP**  | Connection-oriented protocol used for reliable communication (e.g., loading web pages). |
| **UDP**  | Connectionless protocol used for faster communication (e.g., DNS queries, streaming). |
| **QUIC** | Modern UDP-based transport protocol used by services like Google/YouTube for fast, encrypted connections. |

---

## 🔍 Packet Analysis
- **Source IP Address** → Identifies the sender of the packet.
- **Destination IP Address** → Identifies the receiver of the packet.
- **TCP Packets** → Observed during website connections (three-way handshake: SYN, SYN-ACK, ACK).
- **UDP Packets** → Observed mainly for DNS lookups (domain name → IP resolution).
- **QUIC Packets** → Frequently detected, indicating encrypted, UDP-based web communication.

---

## ✅ Result
Network traffic was successfully captured and analyzed using Wireshark. The capture clearly demonstrated how devices communicate over a network using different protocols, and how source/destination addresses route data between systems.

---

## 📝 Conclusion
This task provided hands-on experience with Wireshark for monitoring and inspecting live network traffic. By analyzing **TCP**, **UDP**, and **QUIC** packets, a clearer understanding was gained of how modern web communication occurs — including connection establishment, DNS resolution, and the growing use of encrypted protocols like QUIC for secure browsing. This exercise strengthened foundational skills in **network traffic analysis** and **packet-level inspection**.

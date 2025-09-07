# Analysis of TCP Connection Establishment

### Objective
This analysis demonstrates the fundamental process of a TCP connection—the **three-way handshake**. By capturing live network traffic, this exercise visualizes the theoretical concepts of TCP flags in a practical, real-world scenario.

### Methodology
* **Tool:** Wireshark
* **Action:** A standard TCP connection was initiated by browsing to `http://scanme.nmap.org`, a safe and legal target for security testing, hosted at `45.33.32.156`.
* **Capture:** Wireshark was used to capture the packets exchanged during this session.

### Observation
The screenshot below isolates the three key packets that constitute a successful handshake, identified by their TCP flags:

1.  **[SYN]**: The client sends a **SYN**chronize packet to the server to initiate the connection.
2.  **[SYN, ACK]**: The server responds with a **SYN**chronize-**ACK**nowledgment packet, indicating that it is open and ready to connect.
3.  **[ACK]**: The client sends a final **ACK**nowledgment packet, completing the handshake and officially establishing the connection.

### Conclusion
Successfully capturing and identifying these packets confirms a foundational understanding of TCP/IP communication. This process is a cornerstone of network analysis and is the underlying mechanism for many network scanning techniques used in ethical hacking.<img width="1062" height="41" alt="Screenshot 2025-09-07 233554" src="https://github.com/user-attachments/assets/1ed1e9d6-c5c3-49c7-b171-a4b2922696fa" />

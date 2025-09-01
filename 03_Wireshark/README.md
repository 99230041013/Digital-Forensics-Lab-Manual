# Experiment 3 – Wireshark

**Objective:**  
To capture, filter, and analyze network traffic using Wireshark.

---

## Description  
Wireshark is a widely used open-source network protocol analyzer.  
It allows investigators to capture and interactively browse traffic running on a computer network.  

With Wireshark, forensic analysts can:  
- Capture live network packets.  
- Apply filters to isolate protocols such as HTTP, DNS, or TCP.  
- Analyze suspicious communication patterns.  
- Export captured traffic for reporting.  

It is especially useful in network forensics to identify malicious traffic, detect intrusions, and reconstruct communication sessions.  

---
<img width="1512" height="872" alt="Image" src="https://github.com/user-attachments/assets/340cf38a-d934-426d-9d43-7009e3cbc00e" />


## Procedure  
1. Launch Wireshark and select the active network interface.  
2. Start packet capture.  
3. Apply filters (e.g., `http`, `dns`, `ip.addr==192.168.1.1`).  
4. Analyze captured traffic.  
5. Export relevant packets for further reporting.  

---

## Expected Output  
- Captured packet data (.pcap).  
- Filtered results showing network activity.  
- Insights on suspicious traffic.  

---

## Output Screenshots  
![Wireshark Capture](screenshots/wireshark-capture.png)  
*Figure 1: Capturing live network packets with Wireshark*  

![Wireshark Filter](screenshots/wireshark-filter.png)  
*Figure 2: Applying filters to analyze HTTP traffic*  

# Task 5 – Capture and Analyze Network Traffic Using Wireshark

## Objective
The goal of this task is to perform a live network traffic capture using **Wireshark**, analyze the captured packets, and identify at least three different protocols used in the communication.


## Tools Used
- **Wireshark v4.x**
- **Windows 10** (or Linux-based system)
- **Web Browser** (Chrome)
- **Command Line (cmd)** for generating ping and DNS traffic


## Steps Performed

### 1. Installed Wireshark
Downloaded from [https://www.wireshark.org](https://www.wireshark.org) and installed along with **Npcap** for packet capturing.

### 2. Captured Live Traffic
- Selected the active **Wi-Fi interface**
- Initiated packet capture
- Generated traffic by:
  - Browsing websites: `openai.com`, `example.com`
  - Running terminal commands:
    - `ping google.com`
    - `nslookup openai.com`
- Stopped capture after ~1 minute

### 3. Applied Protocol Filters
Filtered and analyzed packets for the following protocols:
- `http`
- `dns`
- `icmp`

### 4. Saved Capture
- Exported packet capture to file: `task5_capture.pcap`

## Observations
- DNS queries were sent **before** HTTP requests – confirming name resolution occurs before web communication.
- ICMP packets were visible with clear Echo R

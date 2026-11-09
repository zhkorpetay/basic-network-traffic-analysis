# basic-network-traffic-analysis
Beginner cybersecurity project: network traffic analysis using Wireshark.
# Project 01 — Basic Network Traffic Analysis

## About the Project
This is my first beginner cybersecurity project. I used Wireshark to capture and analyze network traffic on my own MacBook.

## Objective
The goal was to understand how network packets work and learn how to identify IP addresses, protocols, and ports.

## Tools
- Wireshark
- macOS
- Wi-Fi network interface (en0)

## What I Did
1. Captured network traffic using Wireshark.
2. Applied DNS, TLS, and UDP filters.
3. Examined packet information.
4. Identified source and destination IP addresses.
5. Analyzed ports and protocols.

## Filters Used
```text
dns
tls.handshake.extensions_server_name
udp.port == 443
```

## Example Packet Analysis

- Packet number: 43133
- Packet size: 73 bytes
- Protocol: QUIC over UDP
- Source IP: 17.250.84.147
- Destination IP: 192.168.0.204
- Source port: 443
- Destination port: 61068

## Findings
- DNS traffic included the domain `aaplimg.com`.
- TLS traffic showed connections associated with ChatGPT and Apple services.
- QUIC traffic over UDP port 443 was observed.
- YouTube was not identified in this capture.

## What I Learned
- How to use basic Wireshark filters.
- How to identify source and destination IP addresses.
- How ports and protocols appear in captured packets.
- The difference between DNS, TLS, UDP, and QUIC.

## Limitations
Not every application or website was identifiable in the captured traffic. Encrypted connections limit the visibility of their contents.

## Author
Beginner Cybersecurity Learner

# Cybersecurity Internship Task 5: Network Traffic Analysis

## Objective
To capture live network packets and identify basic protocols and traffic types using Wireshark.

## Tools Used
* Wireshark

## Identified Protocols
During the 60-second packet capture, I filtered and analyzed the network traffic to identify the following protocols:

1. **HTTP (Hypertext Transfer Protocol):**
   * **Observation:** Captured when browsing `http://neverssl.com`. 
   * **Details:** I could view the GET requests and the plaintext HTML response in the packet details, demonstrating how unencrypted traffic transmits data.
2. **DNS (Domain Name System):**
   * **Observation:** Captured when my system resolved domain names to IP addresses.
   * **Details:** The capture showed Standard Query packets asking for the A (IPv4) records of the websites visited, followed by the server's response packets.
3. **TCP (Transmission Control Protocol):**
   * **Observation:** Present as the underlying transport protocol for HTTP and HTTPS traffic.
   * **Details:** The classic three-way handshake (SYN, SYN-ACK, ACK) was visible when establishing connections with web servers.

## Files Included
* `task5_capture.pcap`: The raw packet capture file containing the analyzed network traffic.

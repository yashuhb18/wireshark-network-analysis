# Network Traffic Analysis using Wireshark

## Objective

To capture and analyze live network traffic using Wireshark and understand the behavior of common network protocols.

## Tools Used

* Wireshark
* Web Browser
* Command Prompt

## Protocols Analyzed

* TCP
* UDP
* ICMP
* HTTPS (TLS)
* DNS

## Key Observations

### TCP

* Three-way handshake (SYN, SYN-ACK, ACK)
* Reliable communication
* Uses ports 80 (HTTP) and 443 (HTTPS)

### UDP

* No handshake
* Faster but less reliable
* Used in DNS (Port 53)

### ICMP

* Used for network diagnostics (ping)
* No port numbers
* Echo request and reply observed

### HTTPS (TLS)

* Data is encrypted
* Only handshake is visible
* Port 443 used

### DNS

* Resolves domain names to IP addresses
* Uses UDP (Port 53)

---

## Analysis of HTTP vs HTTPS Behavior

During this project, the behavior of both HTTP and HTTPS protocols was analyzed using Wireshark to understand how data is transmitted over a network.

### HTTP Analysis

* Captured HTTP POST requests in Wireshark.
* Observed that sensitive information such as usernames and passwords was visible in plaintext.
* Demonstrates that HTTP does not use encryption, making it vulnerable to interception and data exposure.

### HTTPS Analysis

* Captured HTTPS traffic and observed the TLS handshake process.
* Packet contents were encrypted and could not be read in plaintext.
* Demonstrates that HTTPS uses encryption to secure communication between client and server.

### Key Insight

This analysis clearly shows the difference between HTTP and HTTPS in terms of security. While HTTP exposes sensitive data, HTTPS protects it through encryption.

This experiment demonstrates how attackers can intercept unencrypted traffic and highlights the importance of using secure protocols in real-world applications.

## Security Insight
The analysis clearly demonstrates that unencrypted HTTP traffic exposes sensitive information, while HTTPS protects data using encryption. This highlights the importance of secure communication protocols in preventing data interception attacks.

---

## Results

* Successfully captured and analyzed multiple protocols
* Understood packet structure and communication flow
* Observed real-world network behavior

## Detailed Report

Refer to `report.pdf` for complete documentation.

## Disclaimer

This project was conducted in a controlled environment for educational purposes only.

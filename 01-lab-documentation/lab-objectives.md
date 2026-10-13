# Lab Objectives

Source lab: **Lab - Using Wireshark to Examine HTTP and HTTPS Traffic** (Cisco).

## Objectives stated in the lab
1. Capture and view HTTP traffic.
2. Capture and view HTTPS traffic.

## Learning goals
- Identify the network interface and its IP address using `ip address`.
- Capture traffic to a `.pcap` file using `tcpdump`.
- Open a capture in Wireshark and apply display filters.
- Inspect an HTTP `POST` request and its URL-encoded form data.
- Inspect HTTPS traffic on TCP port 443 and examine TLS application data.
- Compare the visibility of HTTP content with encrypted HTTPS application data.

## Required resources
- CyberOps Workstation VM
- Internet connection

## Expected evidence
- Screenshot of the network interfaces and addresses.
- Screenshot of the HTTP capture and `http` display filter.
- Screenshot of the HTTP POST form fields, with any sensitive values obscured.
- Screenshot of the HTTPS capture filtered with `tcp.port==443`.
- Screenshot of TLS/Encrypted Application Data.
- Notes describing only what was actually observed.

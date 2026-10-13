# Lab Instructions

These instructions organize the workflow described in the Cisco lab. Follow your instructor's current directions if your VM or interface differs from the source document.

## Part 1: Capture and view HTTP traffic

1. Start the CyberOps Workstation VM and log in using the credentials supplied for that VM.
2. Open a terminal and identify the interfaces:
   ```bash
   ip address
   ```
3. Confirm the correct interface name. The source lab uses `enp0s3`.
4. Start the capture:
   ```bash
   sudo tcpdump -i enp0s3 -s 0 -w httpdump.pcap
   ```
5. While `tcpdump` is running, open the lab's HTTP demonstration page as described in the course material and perform the demonstration login only if the page is still available and your instructor authorizes it. Do not use real credentials.
6. Return to the terminal and press `Ctrl+C` to stop the capture.
7. Open `httpdump.pcap` in Wireshark.
8. Apply the display filter:
   ```text
   http
   ```
9. Find a `POST` request and inspect **HTML Form URL Encoded** data, if present. Record what is visible without publishing sensitive values.

## Part 2: Capture and view HTTPS traffic

1. Start a new capture:
   ```bash
   sudo tcpdump -i enp0s3 -s 0 -w httpsdump.pcap
   ```
2. While capturing, browse to the NetAcad website specified in the course lab and generate HTTPS traffic. Sign in only if required for your class and never place your credentials in screenshots or public repositories.
3. Stop the capture with `Ctrl+C`.
4. Open `httpsdump.pcap` in Wireshark.
5. Apply the display filter:
   ```text
   tcp.port==443
   ```
6. Select an Application Data packet and inspect the protocol details. Expand the TLS section (older Wireshark versions may label it SSL).
7. Record whether the encrypted application data is readable as plaintext.

## Notes
- The source lab says to change `enp0s3` if your interface has a different name.
- If the HTTPS page reports a secure-connection error, the source lab notes that an incorrect system date/time may be a cause. Verify the system clock before changing it.
- A capture may contain no matching packets if the wrong interface was selected or no relevant traffic occurred during capture.
- Do not upload raw captures publicly unless you have checked them for sensitive data.

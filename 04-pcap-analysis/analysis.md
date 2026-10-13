# PCAP Analysis

Complete this file after inspecting your own captures in Wireshark. Do not fill in packet numbers, IP addresses, or field values from assumptions.

## Capture details

| Item | HTTP capture | HTTPS capture |
|---|---|---|
| Capture filename | `httpdump.pcap` | `httpsdump.pcap` |
| Interface used | _Record observed value_ | _Record observed value_ |
| Capture date/time | _Fill in_ | _Fill in_ |
| Display filter | `http` | `tcp.port==443` |
| Matching packets found | _Fill in_ | _Fill in_ |

## HTTP capture
1. Was an HTTP POST request present? _Fill in._
2. Was **HTML Form URL Encoded** shown in the packet details? _Fill in._
3. Which two form fields were displayed by your capture? Record field names and redact any values that could be sensitive.
4. What other request/response details did you observe? _Fill in._
5. Screenshot filename(s): _Fill in._

## HTTPS capture
1. Did the `tcp.port==443` filter return packets? _Fill in._
2. Did you find a TLS Application Data packet? _Fill in._
3. What protocol section or label appeared in the packet details? _Fill in._
4. Was the encrypted application data readable as ordinary plaintext? _Fill in._
5. Screenshot filename(s): _Fill in._

## Interpretation
Explain the differences supported by your capture. HTTP can expose application content in readable form; HTTPS protects application data with encryption in transit. Packet metadata may still be visible, and HTTPS alone does not prove that a website is trustworthy.

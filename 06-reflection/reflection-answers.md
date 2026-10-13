# Reflection Answers

These draft answers follow the concepts described in the supplied Cisco lab. Adjust them if your instructor expects answers tied to specific observations.

## 1. What are the advantages of using HTTPS instead of HTTP?

HTTPS uses encryption to protect data exchanged between a browser and a website while it is in transit. This makes the application content much harder for someone monitoring the network to read or alter. HTTPS also uses certificates as part of establishing a protected connection.

## 2. Are all websites that use HTTPS considered trustworthy?

No. HTTPS indicates that the connection is protected with encryption and that the browser has established a certificate-based secure connection; it does not guarantee that the website itself is honest or safe. Threat actors can also use HTTPS to conceal their activities, so users should still check that a website is legitimate and trustworthy.

## Capture-based question: What two pieces of information are displayed in the HTTP form data?

The source lab asks the student to inspect the **HTML Form URL Encoded** section of an HTTP POST packet, but the actual values depend on the capture. Record the two fields shown in your own Wireshark packet details. Do not assume the fields or publish any real credentials.

## Capture-based question: What replaces the HTTP section in the HTTPS capture?

Inspect the protocol tree for the selected packet and write down the section label shown by your Wireshark version. The source lab directs you to examine the Secure Sockets Layer (SSL/TLS) section.

## Capture-based question: Is the encrypted application data in plaintext or readable format?

The expected concept is **no**: encrypted HTTPS application data is not ordinarily readable as plaintext in a packet capture without the appropriate decryption material and setup. Confirm the display in your own capture and note any differences.

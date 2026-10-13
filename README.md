# Wireshark HTTP/HTTPS Lab

A structured lab project for capturing and examining HTTP and HTTPS traffic with `tcpdump` and Wireshark, based on the Cisco lab **“Using Wireshark to Examine HTTP and HTTPS Traffic.”**

## Lab objectives
- Capture and view HTTP traffic.
- Capture and view HTTPS traffic.
- Compare what can be observed in an HTTP form submission with encrypted HTTPS application data.
- Record evidence, findings, and reflection answers.

## Repository structure

```text
Wireshark-HTTP-HTTPS-Lab/
├── 01-lab-documentation/
│   ├── lab-instructions.md
│   └── lab-objectives.md
├── 02-command-reference/
│   └── commands.md
├── 03-screenshots/
│   └── .gitkeep
├── 04-pcap-analysis/
│   └── analysis.md
├── 05-findings/
│   └── findings.md
├── 06-reflection/
│   └── reflection-answers.md
├── .gitignore
├── LICENSE
└── README.md
```

## Requirements
- CyberOps Workstation VM (as specified by the lab)
- Internet connection
- `tcpdump`
- Wireshark

The source lab uses the workstation account `analyst` and gives the password `cyberops`. Use those credentials only if they apply to your provided lab VM. The source uses interface `enp0s3`; check your own interface before capturing.

## Quick workflow
1. Read `01-lab-documentation/lab-instructions.md`.
2. Review the commands in `02-command-reference/commands.md`.
3. Save your screenshots in `03-screenshots/`.
4. Record what you actually observe in `04-pcap-analysis/analysis.md`.
5. Summarize evidence in `05-findings/findings.md`.
6. Answer the reflection questions in `06-reflection/reflection-answers.md`.

## Evidence and safety
- Only capture traffic in your own authorized lab environment.
- Do not include real passwords, session cookies, personal data, or account credentials in screenshots or commits.
- The lab's HTTP example uses a demonstration login. Do not enter real credentials into an HTTP website.
- Capture files (`*.pcap` and `*.pcapng`) may contain sensitive data and are ignored by Git by default.
- Do not claim a packet or field was observed unless you verified it in your own capture.

## Status
This repository is a lab template. Add your own screenshots and fill in observations from your packet captures before submitting.

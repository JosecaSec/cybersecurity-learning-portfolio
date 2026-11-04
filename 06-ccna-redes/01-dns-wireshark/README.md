# LAB-01: DNS Traffic Analysis with Wireshark

## Overview

This lab documents the analysis of DNS queries and responses using Wireshark, based on a practical networking exercise.

## Objectives

- Understand the DNS name resolution process.
- Capture and filter DNS traffic using Wireshark.
- Identify DNS queries and responses.
- Analyze source and destination ports and IP addresses.
- Explain the role of UDP in common DNS communications.

## Tools

- Wireshark
- Web browser
- Windows operating system

## Lab Procedure

Documentation in progress.

## Packet Analysis
### DNS Response Analysis
During the lab, DNS traffic was captured and examined using Wireshark.
The following UDP ports were observed in a DNS response packet:

| Field | Observed Value |
|---|---|
| Application Protocol | DNS |
| Transport Protocol | UDP |
| Source Port | 53 |
| Destination Port | 33840 |

### Technical Explanation
The DNS server sends its response using UDP source port 53. The client receives the response on its temporary UDP port 33840, which was used for the corresponding DNS transaction.
This demonstrates how DNS name resolution commonly uses UDP and how transport-layer port numbers identify the communicating application endpoints.
## Evidence

Screenshots and sanitized capture examples will be added.

## Conclusions

Documentation in progress.

## Security Considerations

Only sanitized traffic and non-sensitive information will be published.

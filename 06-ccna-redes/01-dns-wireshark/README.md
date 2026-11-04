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
### Step 1: Prepare the Environment

- Open Wireshark on the Windows computer.
- Select the active network interface.
- Start capturing network traffic.

### Step 2: Generate Network Traffic

- Open a web browser.
- Navigate to a website to generate network activity.
- Return to Wireshark and stop the packet capture.

### Step 3: Filter DNS Packets

- Enter the following display filter in Wireshark:

```text
dns
```

- Apply the filter to identify DNS packets in the capture.
- Locate DNS query and response packets, if present.

### Step 4: Examine DNS Communication

- Select a DNS response packet.
- Expand the Internet Protocol and User Datagram Protocol sections.
- Identify the source and destination ports.
- Review the Domain Name System section to inspect the DNS message.

### Step 5: Record Findings

- Record the observed UDP source port: 53.
- Record the observed UDP destination port: 33840.
- Explain how the DNS response reaches the client through the temporary UDP port.

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

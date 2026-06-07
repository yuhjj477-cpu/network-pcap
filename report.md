# Network Traffic Analysis Report using Wireshark

## Objective

The objective of this task was to capture and analyze live network traffic using Wireshark and identify basic protocols and traffic types.

## Tools Used

* Wireshark
* Packet Capture Format: `.pcap`

## Methodology

1. Started packet capture using Wireshark.
2. Generated network traffic by browsing and network communication.
3. Captured packets for approximately one minute.
4. Applied protocol filters and analyzed packet details.
5. Exported the captured traffic as a `.pcap` file.

---

# Capture Summary

* Total Packets Captured: **32 packets**
* Capture Type: **Ethernet Packet Capture**
* Primary Traffic Type: **UDP-based traffic**

---

# Protocols Identified

## 1. Ethernet (Layer 2)

* All captured packets were encapsulated using Ethernet frames.
* Ethernet provides communication between devices on the local network.

## 2. IPv4 (Layer 3)

* The packets were transmitted using IPv4 addressing.
* Example local IP observed:

`192.168.50.50`

## 3. UDP (User Datagram Protocol)

* Most captured packets used UDP.
* UDP is a connectionless protocol commonly used for lightweight communication.

## 4. DNS Traffic

* DNS packets were detected.

Observed communication:

* Source Port: **1026**
* Destination Port: **53**

This indicates a DNS query/response for hostname resolution.

## 5. NTP Traffic (Network Time Protocol)

Most traffic consisted of NTP communication.

Observed:

* Source Port: **123**
* Destination Port: **123**

This traffic is used for time synchronization between systems.

---

# Packet Analysis Findings

* Majority of traffic was **UDP-based NTP synchronization traffic**
* Small amount of **DNS traffic** was present
* No significant TCP or HTTP traffic was observed
* Local device communicated with multiple external IP addresses

Example external addresses observed:

* 67.129.68.9
* 69.44.57.60
* 207.234.209.181

---

# Conclusion

The packet capture successfully identified multiple network protocols including Ethernet, IPv4, UDP, DNS, and NTP. Analysis showed that the captured traffic primarily consisted of network time synchronization traffic with minor DNS activity.

The objective of capturing and analyzing live traffic using Wireshark was successfully completed.

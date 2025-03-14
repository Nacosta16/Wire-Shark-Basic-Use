# Wire Shark Basic Use and Its Display of the OSI Model

Introduction to Wireshark
Wireshark is a network protocol analyzer used to capture and inspect packets on a network in real-time. It allows network administrators, cybersecurity professionals, and developers to analyze network traffic for troubleshooting, security assessments, and protocol debugging.

Basic Features of Wireshark
Packet Capture – Captures live network traffic.
Packet Filtering – Uses display and capture filters to narrow down traffic.
Packet Analysis – Examines protocol details at different OSI model layers.
Protocol Decoding – Recognizes and interprets hundreds of protocols.
Export & Save Data – Exports captured data for later analysis.
Wireshark and the OSI Model
Wireshark analyzes network traffic at various layers of the OSI (Open Systems Interconnection) model, which is divided into seven layers:

1. Physical Layer (Layer 1)
Represents raw bits on the network medium (e.g., Ethernet cables, fiber optics).
Wireshark does not directly capture physical layer data but can infer issues (e.g., retransmissions).
2. Data Link Layer (Layer 2)
Deals with MAC addresses and Ethernet frames.
Wireshark captures Ethernet frames, VLAN tags, and ARP packets.
Example filter: eth.addr == 00:1A:2B:3C:4D:5E (Filters packets from a specific MAC address).
3. Network Layer (Layer 3)
Handles IP addressing and routing (IPv4, IPv6).
Wireshark captures IP packets and ICMP messages (e.g., ping).
Example filter: ip.src == 192.168.1.1 (Shows packets from a specific IP).
4. Transport Layer (Layer 4)
Manages TCP/UDP communications.
Wireshark inspects TCP handshakes, UDP streams, and port-based filtering.
Example filter: tcp.port == 80 (Filters HTTP traffic).
5. Session Layer (Layer 5)
Manages sessions and connections (e.g., SSH, SMB).
Wireshark helps track session initiation and termination.
Example filter: tcp.stream eq 1 (Follows a single TCP conversation).
6. Presentation Layer (Layer 6)
Deals with data encryption and encoding (e.g., SSL/TLS).
Wireshark captures SSL/TLS handshakes and encrypted traffic.
Example filter: ssl (Displays SSL/TLS traffic).
7. Application Layer (Layer 7)
Represents end-user applications like HTTP, FTP, DNS, and SMTP.
Wireshark can reconstruct web browsing sessions and detect anomalies.
Example filter: http.request (Shows all HTTP requests).

# Wire Shark Basic Use and Its Display of the OSI Model

  <h2> Basic Features of Wireshark </h2>
  
 - <b> Packet Capture – Captures live network traffic </b>

 - <b> Packet Filtering – Uses display and capture filters to narrow down traffic </b>

 - <b> Packet Analysis – Examines protocol details at different OSI model layers </b>

 - <b> Protocol Decoding – Recognizes and interprets hundreds of protocols </b>

 - <b> Export & Save Data – Exports captured data for later analysis </b>

  <h2> Wireshark and the OSI Model </h2>

  Wireshark analyzes network traffic at various layers of the OSI (Open Systems Interconnection) model, which is divided into seven layers:

1. Physical Layer (Layer 1)
Represents raw bits on the network medium, such as ethernet cables, fiber optics, but Wireshark does not directly capture physical layer data but can infer issues
3. Data Link Layer (Layer 2)
Deals with MAC addresses and Ethernet frames
Wireshark captures Ethernet frames, VLAN tags, and ARP packets

4. Network Layer (Layer 3)
Handles IP addressing and routing (IPv4, IPv6)
Wireshark captures IP packets and ICMP messages, like using ping

5. Transport Layer (Layer 4)
Manages TCP/UDP communications
Wireshark inspects TCP handshakes, UDP streams, and port-based filtering

6. Session Layer (Layer 5)
Manages sessions and connections auch as SSH
Wireshark helps track session initiation and termination.

7. Presentation Layer (Layer 6)
Deals with data encryption and encoding such as SSL/TLS
Wireshark captures SSL/TLS handshakes and encrypted traffic.

8. Application Layer (Layer 7)
Represents end-user applications like HTTP, FTP, DNS, and SMTP
Wireshark can reconstruct web browsing sessions and detect anomalies


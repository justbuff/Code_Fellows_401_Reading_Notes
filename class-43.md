# What Is a Sniffing Attack?

A sniffing attack can be performed using an application or hardware devices at both the network and host level. Any network packet having information in plain text can be intercepted and read by the attackers. This information can be usernames, passwords, secret codes, banking details or any information which is of value to the attacker. 

There are two types of sniffing:

Passive sniffing: This kind of sniffing occurs at a hub, where the sniffer can sit undetected and spy on the network. Since hubs are not used these days much, this kind of attack will be an old-school trick to perform. 

Active sniffing: The sniffer will flood the switch with bogus requests so that the CAM table (where the destination MAC addresses are stored) gets full. Once the CAM is full the switch will act as a switch and send the network traffic to all ports where it is sniffed. 

Sniffing attack implementations: MAC flooding, DNS cache poisoning, Evil twin attack, and MAC spoofing.

Protocols vulnerable to sniffing attacks: HTTP, Telnet, FTP, POP, and SNMP.

Precautionary measures against Sniffing attacks:

- Connect to trusted networks

- Encrypt all the traffic that leaves your system.

- Network scanning and monitoring

Reference: https://www.greycampus.com/blog/information-security/what-is-a-sniffing-attack-and-how-can-you-defend-it

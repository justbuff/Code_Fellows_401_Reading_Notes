# Intrusion Detection and Prevention Systems (IDS/IPS)

An IDS is a visibility tool that sits off to the side of the network and monitors traffic and consists of a management console and sensors. When the sensors encounter something that matches up to a previously detected attack signature, they report the activity to the console. An IDS can notify security personnel of infections, spyware or key loggers, as well as accidental information leakage, security policy violations, unauthorized clients and servers, and even configuration errors.

An IPS is similar to an IDS, except that they are able to block potential threats as well. They monitor, log and report activities, similarly to an IDS, but they are also capable of stopping threats without the system administrator getting involved.

A Network Intrusion Detection System (NIDS) and a Host Intrusion Detection System (HIDS) are complementary systems that differ by the position of the sensors: network-based (monitoring the ethernet or WiFi) and host-based, respectively. Network-based sensors have a quicker response than host-based sensors and they are also easier to implement. A NIDS can also detect attacks that an HIDS will miss because it looks at packet headers in real-time.

Pros of Network Intrusion Detection Systems

- They Can Be Tuned to Specific Content in Network Packets

- They Can Look at Data in the Context of the Protocol

- They Can Qualify and Quantify Attacks

- They Make It Easier to Keep Up With Regulation

- They Can Boost Efficiency

Cons of Network Intrusion Detection Systems

- They Will Not Prevent Incidents By Themselves

- An Experienced Engineer Is Needed to Administer Them

- They Do Not Process Encrypted Packets

- IP Packets Can Still Be Faked

- False Positives Are Frequent

- They Are Susceptible to Protocol Based Attacks

- The Signature Library Needs to Be Continually Updated to Detect the Latest Threats

### Cyber Security Attack Vectors
- **Cloud Computing Threats** - Cloud computing is an on-demand delivery of IT capabilities in which IT infrastructure and applications are provided to subscribers as a metered service over a network. 
- **Advanced Persistent Threat** - Advanced persistent threat is a threat that focuses on stealing information from the victim machine without its user being aware of it. APTs exploit vulnerabilities in the applications running on a computer, operating system, and embedded systems.
- **Viruses and Worms** - Viruses and worms are the most prevalent networking threats, capable of infecting a network within seconds. A virus is a self-replicating program that produces a copy of itself by attaching to another program, computer boot sector, or document.
- **Ransomware** - Ransomware is a type of malware, which restricts access to a computer system’s files and folders and demands an online ransom payment to the malware creator(s) to remove the restrictions.
- **Mobile Threats** - Attackers are increasingly focusing on mobile devices due to the increased adoption of smartphones for business and personal use and their comparatively fewer security controls. Users may download malware applications (APKs) onto their smartphones, which can damage other applications and data and convey sensitive information to attackers. 
- **Botnet** - A botnet is a huge network of compromised systems used by attackers to perform denial-of-service attacks. Bots, in a botnet, perform tasks such as uploading viruses, sending emails with botnets attached to them, and stealing data. 
- **Insider Threat** - An insider threat can be used to launch an attack by someone from within an organization who has authorized access to its network and is aware of the network architecture.
- **Phishing** - Phishing is a practice of sending an illegitimate email falsely claiming to be from a legitimate site to acquire a user’s personal or account information.
- **Web Application Threats** - Web application attacks like SQL injection and cross-site scripting have made web applications a favorable target for the attackers to steal credentials, set up a phishing site, or acquire private information.
- **IoT Threats** - The IoT devices connected to the Internet have little or no security, which makes them vulnerable to various types of attacks. These devices include many software applications that are used to access the device remotely.


### Opportunity-Vulnerability-Weakness
#### TCP/IP Protocol Vulnerabilities  
- The TCP/IP is one of the most widely used protocol suites, but it is vulnerable to attack due to various security flaws inherent in it. These flaws are present because hosts depend only on IP source address for authentication, while other flaws are present because network control mechanisms and routing protocols have less or no authentication. 
#### Operating System Vulnerabilities
- An operating system is vulnerable if it is inherently insecure or if it is not updated. For example, some common types of vulnerabilities found in Windows-based machines are Memory corruption, Overflow, Remote Code Execution, DoS, and CSRF File inclusio
#### Network Device Vulnerabilities
- Organizations depend upon various network devices, such as routers, firewalls, and switches, to make communication among the mail servers and web servers.

## Understand Network Attack Tactics, Techniques, and Procedures (TTPs)
### Reconnaissance Attacks
- **Examples** - Packet Sniffing, Port scanning, Ping sweeping, DNS footprinting, Social engineering
### Network Scanning 
- Nmap is a network discovery and security-auditing tool and is one of the most popular tools attackers use for network discovery. An attacker mostly uses the Nmap utility to extract all the necessary information from the target.
### Port Scanning
- Port scanning is the process of checking what services are running on the target computer by sending a sequence of messages to break in. Port scanning involves connecting to or probing TCP and UDP ports on the target system to determine if the services are running or are in a listening state. The listening state provides information about the operating system and the application currently in use.
### DNS Footprinting
- DNS footprinting reveals information about DNS zones. DNS zone data includes the DNS domain names, computer names, IP addresses, and much more about a particular network. An attacker uses the DNS information to determine key hosts in the network, and then performs social engineering attacks to gather even more information.
### Network Sniffing
- Internal Sniff,  External Sniff, Wireless Sniff
### Man-in-the-Middle Attack
- A man-in-the-middle attack (also known as MiTM) is a type of attack in which attackers intrude into an existing connection between two systems to intercept the messages being exchanged and to inject fraudulent information.
### Password Attacks
#### Password Attack Techniques 
-  Dictionary Attack, Brute Forcing Attack, Hybrid Attack,  Birthday Attack,  Rainbow Table Attack
### Privilege Escalation 
- Horizontal Privilege Escalation, Vertical Privilege Escalation
### DNS Poisoning
- DNS poisoning is a process in which the user is misdirected to a fake website by providing fake data to the DNS server. The website looks like a genuine site, but it is controlled by the attacker. It is also called a DNS spoofing attack in which the attacker tries to redirect the victim to a malicious server instead of the legitimate server.
### DNS Cache Poisoning
- The DNS system uses cache memory to hold the recently resolved domain names. It is populated with recently used domain names and respective IP address entries.
-  When the user request is received, the DNS resolver first checks the DNS cache; if the domain name that the user requested is found in the cache, then the resolver sends its respective IP address quickly, reducing the traffic and time for DNS resolving.

<img width="867" height="452" alt="image" src="https://github.com/user-attachments/assets/4e879c6e-09d1-40be-8cd6-b5f03f9a9589" />

### ARP Poisoning
- ARP poisoning is an attack in which the attacker tries to associate their own MAC address with the victim’s IP address so that the traffic meant for that IP address is sent to the attacker. ARP (Address Resolution Protocol) is a TCP/IP protocol that maps IP network addresses to the addresses (hardware addresses) used by the data link protocol. Using this protocol, attackers can easily get the MAC address of any device within a network.

<img width="897" height="442" alt="image" src="https://github.com/user-attachments/assets/fd6a653d-4b11-47a0-8b11-2611e78c3f32" />

### DHCP Starvation Attacks
- In a DHCP starvation attack, an attacker floods the DHCP server by sending many DHCP requests and uses all the available IP addresses that the DHCP server can issue. As a result, the server cannot issue any more IP addresses, leading to a denial of service (DoS) attack. Because of this issue, valid users cannot obtain or renew their IP addresses, and thus fail to access their network.

<img width="876" height="424" alt="image" src="https://github.com/user-attachments/assets/3a16660f-ba87-4d97-a403-ec033b19976d" />

### DHCP Spoofing Attack
- A DHCP Spoofing attack is also known as a rogue DHCP server attack. In a rogue DHCP server attack, an attacker will introduce a rogue server in the network. This rogue server could respond to client’s DHCP discovery requests. Though both the servers respond to the request, that is, the rogue server and the actual DHCP server, the server that responds first will be taken by the client. If the rogue server gives the response earlier than the actual DHCP server, the client takes the response from the rogue server instead. The information provided to the clients by this rogue server can disrupt their network access, causing a DoS.

<img width="929" height="401" alt="image" src="https://github.com/user-attachments/assets/464bd340-8778-430d-a780-55dad79eabfc" />

### Switch Port Stealing
- Switch port stealing is a sniffing technique used by an attacker who spoofs both the IP address and MAC address of the target machine. Using a port stealing attack, attackers steal traffic destined to a specific port of an Ethernet switch. It allows an attacker to sniff the packets that were originally destined for another computer. An attacker takes advantage of a switch’s incapability of updating its address table dynamically. Ethernet switches learn and maintain information about who is connected to the port. This information includes the IP and Mac addresses of the computers connected to the network.

<img width="874" height="381" alt="image" src="https://github.com/user-attachments/assets/d31203db-c236-4a11-bc13-32bfdd13f0ad" />

### MAC Spoofing/Duplicating
- Spoofing attacks allow attackers to spread malware, bypass authentication checks, or steal sensitive information. The attacker pretends to be a legitimate user on a network and gets access to restricted resources to perform malicious activities. MAC duplicating refers to spoofing the MAC address with the MAC address of a legitimate user on the network. It involves sniffing a network for the MAC addresses of legitimate clients connected to the network. In this attack, the attacker first retrieves the MAC addresses of clients who are actively associated with the switch port. 

<img width="885" height="361" alt="image" src="https://github.com/user-attachments/assets/4b624876-5a26-426f-b120-8fc01a094e72" />


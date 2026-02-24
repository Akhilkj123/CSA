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




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

### Network-based Denial-of-Service Attack (DoS) 
- In network-based DoS attack, the attacker sends a large amount of traffic to target network than the victim network can handle, thereby exhausting the victim’s connection resources. Attacker does it by exploiting the existing implementation of network protocols.
#### TCP SYN Flooding
- In a TCP SYN attack, the attacker sends a succession of SYN requests to a target's system to make the system unavailable for legitimate users. It exploits a known weakness in the TCP connection.
#### UDP Flooding
- In UDP flooding attack, an attacker sends multiple user datagram protocol (UDP) packets to the targeted server with the aim of making it unable to process and respond. In normal situations, on receiving a UDP packet at a specific port, a server first validates whether any program is running at that port to respond to the request. If no program is found at that port, then a server will send ICMP (ping) packet to acknowledge the client that the destination is inaccessible.
#### ICMP Smurf Flooding 
- In ICMP smurf flooding attack, an attacker sends multiple ICMP Echo request packets to the targeted server with the aim of making it shut down. This type of attack makes use of an IP broadcast network function, where an ICMP Echo (ping) request is sent to every host, to get instant response from each receiver
#### Intermittent Flooding
- The intermittent flooding attack is an application layer DDoS attack. It is also known as Very Short Intermittent DDoS attack. In this type of attack, an attacker transmits intermittent floods of valid HTTP requests to the victim system, to obtain unsaturated DoS.

### Distributed Denial-of-Service Attack (DDoS)
- A distributed denial-of-service (DDoS) attack is a large-scale, coordinated attack on the availability of services on a target’s system or network resources. It is launched indirectly through many compromised computers on the Internet. The services under attack are those of the “primary target,” while the compromised systems used to launch the attack are often called the “secondary target.” The use of secondary targets in performing a DDoS attack provides the attacker with the ability to wage a larger and a more disruptive attack, while making it more difficult to track them.
####  Network-centric attack
- A network-centric attack targets the bandwidth of a network or service by flooding the network infrastructure with an immense volume of traffic. This overwhelms routers, switches, and other network components, thereby consuming the network's bandwidth capacity. 
#### Application-centric attack
- An application-centric DDoS attack targets the application layer of a service or server. Attackers send a high volume of requests or transactions to specific applications or services hosted on servers.

### Malware Attacks
- Malware is a piece of malicious software that is designed to perform activities as intended by the attacker without user consent. It appears in the form of executable code, active content, scripts, or other forms of software. The attacker compromises system security, intercepts computer operations, gathers sensitive information, modifies, delete or add content to a website, take control of a user’s computer, and so on.
#### Virus
- A virus is a type of program that can duplicate itself by making copies of itself. The major criterion for categorizing a piece of executable code as a virus is that it replicates itself through hosts. A virus can only spread from one PC to another when its host is taken to the uncorrupted computer.
#### Armored Virus
- An armored virus is a type of computer virus that is specifically coded with different mechanisms to make its detection difficult. It fools antivirus programs, making them believe the armored virus is located somewhere else in memory and making it difficult to detect and remove.
#### Trojan
- A Trojan is a malicious program that masquerades as legitimate software. A Trojan horse attack is termed as a “serious threat to system security.” A victim may be under attack from the Trojan, but they could also be used as an intermediary to attack others (without the knowledge of the victim). Most Trojans consist of two parts: server and a client. A server is a program that gets installed on the infected system. The client is also a program that is located on the attacker’s computer. Both the server and client are used to establish a connection between the attacker and a victim’s system via the Internet.
#### Adware
- Adware is a software program that tracks the user’s browsing patterns for marketing purposes and displaying advertisements. It collects the user’s data, such as what types of Internet sites the user visits in order to customize the adverts that are relevant to the user. Legitimate software is embedded with adware programs to generate revenue.
#### Spyware
- Spyware is a piece of software code that extracts the user’s information and sends it to attackers. It enables pop-up advertisements to appear, modifies computer settings, redirects users to fake webpages or changes the home page of the browser. Users are not aware of spyware being installed on their computer. Most of the time, spyware is used to track cookies and display unwanted pop-up ads. Its presence is hidden from the user, and it is difficult to detect.
#### Rootkits
- Rootkit is a software program that hides its activities from detection and performs malicious activities to get privileged access to a target computer. It hides the fact that the operating system is compromised by the attackers. A successful rootkit can potentially remain in place for years if it remains undetected.
#### Backdoors
- Attackers create backdoors to compromise the security of the target systems and gain access to a network illegitimately. Attackers insert small programs that bypass the authentication check such as gaining administrative privileges without passwords. The attacker installs programs and controls the victim’s computer remotely. Attackers use backdoors to get access to a network and keep returning by using the same exploit.
#### Logic Bomb
- A logic bomb is a piece of software code that performs a malicious action when a logic condition is satisfied. When a logic bomb explodes, it unauthentic message, delete data or completely reformat hard drives, send sensitive information to untrusted parties, disable a network for a certain length of time, and cause harm to the target computer.
#### Botnets
- A botnet is a collection of compromised computers connected to the Internet to perform a distributed task. Attackers distribute malicious software that turns a user’s computer into bots. A bot refers to a program or an infected system that performs repetitive work or acts as an agent or as a user interface to control other programs.
#### Ransomware
- Ransomware is a type of malicious software that locks or encrypts valuable files available in the victim’s computer until a ransom is paid. Unlike other malwares, it does not hide, and it displays a message on the infected system that “your files are taken away for ransom and you need to pay money in order to decrypt it.” It redirects victims to different sites and provides information regarding how to make payment to recover the data back. During payment, attackers often collect credit card details that may result in further financial losses.
#### Polymorphic Malware
- Polymorphic malware is a destructive and intrusive malware code that changes its signature to avoid pattern matching detection by antivirus programs. The functionality remains the same even though its signature changes. For example, a spyware program working as a keylogger continues to perform the same action, even if its signature changes.

### Advanced Persistent Threats (APTs)
- In Advanced persistent threat, the attacker gains unauthorized access to a target network and remains there undetected for a long period of time. In APT, the word “advanced” signifies the use of techniques to exploit the underlying vulnerabilities in the system. The word “persistent” signifies the external command and control (C&C) system that continuously extracts the data and monitors the victim’s network. T

#### Characteristics of Advanced Persistent Threats (APTs)
- Objectives, Timeliness, Resources, Risk Tolerance, Skills and Methods,  Actions, Attack Origination Points, Numbers Involved in the Attack,  Knowledge Source,  Multiphase, Tailored to the Vulnerabilities, Multiple Points of Entries, Evading Signature-based Detection Systems


  
  




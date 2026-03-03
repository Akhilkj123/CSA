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

#### Advanced Persistent Threat Lifecycle 
- In the current threat landscape, organizations need to concentrate more on APTs. Advanced persistent threats may target an organization’s IT assets, financial assets, intellectual property, and reputation.

<img width="811" height="479" alt="image" src="https://github.com/user-attachments/assets/0b64b920-404e-47c2-b8d1-d50f335453df" />

### Supply Chain Attack
- A supply chain attack is a type of cyberattack in which an attacker infiltrates an organization's network by targeting its suppliers, third-party vendors, or elements within the supply chain. The supply chain encompasses a complex and interconnected network involving individuals, organizations, resources, activities, and technology, all working together in the production and distribution of products.
#### Working of Supply Chain Attack
- Attackers often compromise third-party vendors' software to gain unauthorized access to the supply chain, subsequently distributing malware within the network, which can lead to data breaches. Typically, attackers focus on targeting third parties with perceived weaker cybersecurity measures. Once they identify the weakest link in the supply chain, they concentrate their efforts on launching a supply chain attack against the ultimate target. 

<img width="320" height="410" alt="image" src="https://github.com/user-attachments/assets/e5cca154-bc43-4dbe-b137-3d98dae38da9" />

<img width="976" height="410" alt="image" src="https://github.com/user-attachments/assets/af48d74f-7460-4e6a-8e78-72db675a7093" />

<img width="1004" height="442" alt="image" src="https://github.com/user-attachments/assets/a750f043-4ee9-49ba-ac6f-f8038e198fdc" />

## Understand Host Attack Tactics, Techniques, and Procedures (TTPs)
### Common Threats Specific to Host Security
#### Malware Attack (Infection) 
- Viruses, Worms, Worms, Spyware, Backdoor, Ransomware, Adware, Rootkits, Fileless malware.

#### Unauthorized Access
- Unauthorized access refers to gaining unauthorized access to restricted files, data, operation, services, and so on running on host. These attacks are designed to bypass security measures and gain access to sensitive data, critical system functions, or other restricted areas of a host.
#### Brute Force Attacks
- A brute force attack is a method used by attackers to gain unauthorized access by systematically trying all possible combinations of passwords or encryption keys until the correct one is found. This attack exploits weak passwords or poorly secured authentication systems, where attackers use automated tools to generate and test vast numbers of possible passwords at high speed.
#### Privilege Escalation
- Privilege escalation attacks occur after an attacker gains unauthorized access through methods like brute force, where they might to the complete takeover of critical initially have limited user privileges. By exploiting vulnerabilities within the host system, such as software bugs, configuration errors, or unpatched security flaws, the attacker can escalate their privileges to gain administrative or root-level access.
#### Host-based DoS attacks
- In host-based DoS attack, the attacker exhausts vulnerabilities in the implementation of the victim’s system’s OS, memory
resources by exploiting algorithms, structure, authentication protocols, and so on. 
- **Ping of Death** - In ping implementation, the maximum accepted size of IP packet is 65535 bytes. This IP packet comprises packet header of 20 bytes and pseudo header of 8 bytes. Thus, 65507 bytes (65535-20-8 = 65507) is the maximum accepted size of an ICMP Echo request

<img width="851" height="120" alt="image" src="https://github.com/user-attachments/assets/9a77f0b0-c3a2-4f4e-b41f-edec67356cdc" />

- **Teardrop Attack** - The IP header contains multiple fields, among which one is “fragment offset” field. This field specifies that the offset means beginning point of a particular fragment correspond to actual unfragmented IP datagram.

<img width="878" height="528" alt="image" src="https://github.com/user-attachments/assets/dd343136-6d8f-4cfa-bb84-95838be65a0b" />
#### Brute-Force Attacks
- A brute-force attack is a systematic method of attempting to gain unauthorized access to a system by exhaustively trying all possible combinations of passwords or encryption keys.
<img width="830" height="193" alt="image" src="https://github.com/user-attachments/assets/6090bf74-465c-4d12-a0d6-dd28fbcc53a8" />

#### Spyware Attacks
- Spyware is designed to operate stealthily, often going undetected for extended periods. The primary tactic of a spyware attack is to infiltrate the host system without alerting the user or security mechanisms. Spyware can capture a wide range of information, including keystrokes (keylogging), screenshots, browser history, passwords, and financial details
<img width="726" height="250" alt="image" src="https://github.com/user-attachments/assets/a0e5d1a5-2ae7-452e-a45c-9d1a84425f5d" />

#### Ransomware Attacks
- Ransomware attacks are a prevalent and highly destructive form of cyber threat, characterized by the encryption of a victim's data or system, followed by a demand for ransom payment in exchange for the decryption key. The coercion tactic is the core of a ransomware attack. 
<img width="926" height="232" alt="image" src="https://github.com/user-attachments/assets/fd616543-f515-4d46-a6d8-550053827112" />

#### Where Do They Come From?
-  Un-patched computers,  Email, Network file sharing,  Internet downloads, Social engineering, Blended threats

#### SQL Injection Attacks
- SQL injection attacks use a series of malicious SQL queries or SQL statements to directly manipulate the database. Applications often use SQL statements to authenticate users to the application, validate roles and access levels, store, obtain information for the application and user, and link to other data sources.

<img width="982" height="331" alt="image" src="https://github.com/user-attachments/assets/4af1867a-e6d3-4ea4-b045-2e6c26f45da3" />

#### Cross-site Scripting (XSS) Attacks
- Cross-site scripting ('XSS' or 'CSS') attacks exploit vulnerabilities in dynamically generated web pages, which enable malicious attackers to inject client-side script into web pages viewed by other users. It occurs when invalidated input data is included in dynamic content that is sent to a user’s web browser for rendering.
- **How XSS Attacks Work** - A web page consists of text and HTML markup, created by the server, and obtained by the client browser. Servers can control client's interpretation about the statically generated pages but cannot completely control client's interpretation about the output of the page generated dynamically by the servers. Thus, if the attackers insert untrusted content into a dynamic page, neither the server nor the client recognizes it. Untrusted input can come from URL parameters, form elements, cookies, databases queries, and so on.
<img width="882" height="518" alt="image" src="https://github.com/user-attachments/assets/1a23f244-0789-436e-b909-83519df3b219" />

- **Cross-Site Scripting Attack Scenario: Attack via Email** - In a cross-site scripting attack that employs email, the attacker crafts an email that contains a link to malicious script and sends it to the victim, luring the victim to click the link containing the malicious script/query.
<img width="920" height="379" alt="image" src="https://github.com/user-attachments/assets/80fdd275-1803-4807-86d6-98edff3f98ce" />
<img width="859" height="482" alt="image" src="https://github.com/user-attachments/assets/6c54e8fe-f086-4234-b72a-6651f7c5f276" />
<img width="858" height="488" alt="image" src="https://github.com/user-attachments/assets/7f8e25f8-10b5-4c97-b939-b4ac572f6a2a" />
<img width="949" height="564" alt="image" src="https://github.com/user-attachments/assets/ec62c1ce-5060-4096-af75-dbc0bfa346a7" />

- **XSS Attack in Blog Posting** - The attacker finds XSS vulnerability in the techpost.org website, constructs a malicious script <script>onload=window.location='http://www.certifiedhacker.com‘</scrip t>, and adds it in the comment field of TechPost. This malicious script posted by the attacker is stored on the web-application database server and runs in background.
<img width="940" height="500" alt="image" src="https://github.com/user-attachments/assets/9b4da9ac-7410-4522-8c39-2d34cf76a5e0" />

- **XSS Attack in Comment Field** - Many web applications use HTML pages that dynamically accept data from different sources. One can change the data in the HTML pages according to the request. Attackers use HTML web page tags to manipulate data. They launch the attack by changing the comments feature using malicious script.
<img width="940" height="486" alt="image" src="https://github.com/user-attachments/assets/dffda502-6ebd-45cb-a217-fe17d760caa8" />

#### Cross-site Request Forgery (CSRF) Attack
- Cross-Site Request Forgery (CSRF) attack is also known as one-click attack or session riding or XSRF. In this type of attack, a malicious entity forces an end user to perform activities on behalf of the hacker. The level of authority that an end user has decides the effects of the attack. If the end user is a normal user, then the successful CSRF attack forces the end user to perform state changing requests like fund transfer and changing email address.

<img width="888" height="452" alt="image" src="https://github.com/user-attachments/assets/44d9f65f-2e1f-4347-8345-2ecc31937582" />
<img width="966" height="602" alt="image" src="https://github.com/user-attachments/assets/d8f2e61b-5932-4b89-a9cc-a0e866f1814e" />

#### Application-level DoS Attack
- A denial-of-service (DoS) attack is an attack on the availability of a service that reduces, restricts, or prevents accessibility of system resources to its legitimate users. The DoS attack mainly targets the application level because it is difficult to identify and detect attacks at the application level.
- User registration DoS, User enumeration, Login attacks, Account locks out attacks

#### Session Attacks: Cookie Poisoning Attacks
- Cookie poisoning is a kind of parameter tampering attack, in which the attacker modifies the cookie contents to draw unauthorized information about a user and thereby perform identity theft. Cookies frequently transmit sensitive credentials from client browser to server. Attackers can modify these with ease to gain access to the server or assume the identity of another user.

<img width="937" height="443" alt="image" src="https://github.com/user-attachments/assets/a9dc4616-8d75-4480-a19a-11259bbabb2c" />


### OWASP Top 10 Web Application Security Risks
- Broken Access Control, Cryptographic Failures,  Injection, Insecure Design, Security Misconfiguration, Vulnerable and Outdated Components,  Identification and Authentication Failures,  Software and Data Integrity Failures, Security Logging and Monitoring Failures, Server-Side Request Forgery (SSRF).

#### Email Attacks: Phishing
#### Email Attacks: Malicious Email Attachments
#### Email Attacks: Malicious User Redirection
- Emails may contain links, which on clicking may redirect the user to websites hosting malware.(Referrer based, User agent based, Cookie based, OS based
#### Email Attacks: Spamming

### Insider Attacks
- Malicious insider, Negligent insider, Compromised insider

### Espionage Attack
- An espionage attack involves insiders leaking confidential or sensitive information to external parties, such as competitors or foreign agents.
- Information leakage, External parties
### Malicious Software Installation
- Installation of malware/spyware, Compromising systems and stealing information

<img width="795" height="441" alt="image" src="https://github.com/user-attachments/assets/6d8800c9-9c7b-44ad-8df7-1fc46015b936" />

### Network Attack IoCs
- Network indicators are useful for command and control, malware delivery, identifying details about the operating system, browser type, and other computer-specific information.

<img width="1045" height="780" alt="image" src="https://github.com/user-attachments/assets/540c7430-94a2-40df-bcff-452dde4e92d3" />
<img width="1046" height="350" alt="image" src="https://github.com/user-attachments/assets/9127ec76-1537-4bed-a389-f71ad350e336" />

### Host Attack IoC’s
- Host-based indicators are found by performing analysis on the infected system within the organizational network.

<img width="884" height="683" alt="image" src="https://github.com/user-attachments/assets/2fefd4db-1bdb-441b-a355-4a9d02894c4f" />
<img width="889" height="488" alt="image" src="https://github.com/user-attachments/assets/99387d64-7716-4eda-9b3d-dd9957cf395d" />

### Application Attack IoC’s 












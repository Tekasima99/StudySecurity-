# INTRODUCTION TO NETWORK DEVICES [PART 1]

- Open System Interconnection model
- Basic Network Devices

## Open System Interconnection model:

Was developed way to help disparate computing systems communication with each other.
Security can be place in various layers of OSI model to create a layered security arrangement that will improve the security of an overall performance

### OSI LAYER:
```markdown
layer 7 = Application
Layer 6 = Presentation
Layer 5 = Session
Layer 4 = Transport
Layer 3 = Network
Layer 2 = Data Link
Layer 1 = Physical
```
## Basic Network Devices
### - Switch.

> Utilized as an Application-Specific Integrated Circuit(ASIC) and considered as LAYER 2 OSI device:
 1. ASIC chip has specific programing that allow switch to learn when a device is on the network and which ports it is connected to cia that device's layer 2 MAC address.
> Managed switches allow for security to be placed on inviduals switch ports and creating more secure enviroment in networking
> Switch only communicate with local network devices.

### - Wireless Access Point(WAP).

> WAP is a specific type of network that connect wireless network segments with wired network segments and considered as as layer 2 OSI device:
  1. Wireless network segments WAP bridges (802.11)
  2. Ethernet network segments (802.3)
> WAP are capable to utilizing encyrption to help esure a secure network networking enviroment.
> WAP only communicate with local network devices

### - Multilayer Switch (MLS).

> MLS provides normal layer 2 network switching services, but also provide layer 3 or higher OSI model services.
> Most common MLS is a layer 3 switch.
> MLS commonly implements security at layer 2 and higher on OSI model.

### - Router.

> Most common network device for connecting different network together utilizing the layer 3 OSI model logical network information.
> Router uses software programming for decision making, as compared to the switches use of an ASIC chip.
> Firewall and ACL usually placed on router to help secure networks

### - Firewall.

> Can be placed on router or host (software based) or  can be its own device(network appliance)
> It function on multiple layer of OSI model layer(2,3,4,7).
> Block packet from entering and leaving the network:
 1. Stateless Inspection, which examine every packet that against a set of rule. When packet matches a rule, the rule is enforced and the specified action is taken.
 2. Stateful Inspection, which the firewall only examine the state of the connection between networks specially when a connection is made from an internal network to an external network, the firewall will not examine any packets running from the external connection. As a general rule, external connetion not allowed to be initiated with the internal network.
> First line of defense.

### - Load Balancer.

> May also be called a content switch or content filter:
 1. Can be implemented to increase the security of the network by limiting or filtering the content that is allowed.
> A network appliance taht used to load balance between multiple hosts that contain the same data spreading out the workload for greater efficiency.
 1. Used to distribute the requests(workload) to a server farm among the various servers that help no single server gets overload.

### - Proxy Server.

> Is an appliance that requests resources on behalf of client machines.
> Often used to retrieve resources from untrusted ousider network on behalf of the requesting client.
> It hides and protects the requesting client.
> Can be utilized to filter allowed content.
> Can be increase performance by caching commonly requested web pages.

# INTRODUCTION TO NETWORK DEVICES [PART 2]

- Introducing the layered Security Concept.
- Network devices.

## Introducing the Layered Security Concept

> Modern networks are composed with multiple layers of devices ans applications, which lead to security issues:
 1. Each layer or device can contain its own security methods. This means that if a breach occurs in one area of network, the rest of the network will remain secure. It is the best practice to use a layered approach when implementing network security.
> Many security devices are trigered by a specific action occurring (network packet crosses an interface):
 1. Some devices are capable of application awareness and this features allows security devices to make better desicion based on which applications are allowed to operate on network and which application are not allowed to cross through it.
 2. This another layer are allowed to cross through it.
 3. Some devices for application aware include firewalls, proxy servers, and network intrusion detection/prevention system.
 
## Network Devices
 
### Virtual Private Network (VPN)
 
 > VPN will facilitate multiple secure VPN connections to a network.
 > The type of VPN will determine what tunnelling and encryption the VPN concentrator will implement.
 > Most concentrator can function at multiple layer of the OSI model (Layer 2,3 and 7).
 > Outside of internet transaction which use SSL VPN connection (Layer 7) and concentrator will function on layer 3 of OSI model that provide IPsec encryption though a secure tunnel.
 
### Network Intrusion Detection System (NIDS) 

> Is a passive system designed to identify when a network breach or attack against the network occur:
  1. usually designed to inform a network administrator when breach is occur.
  2. The file will send throgh log files, SMS, and/or an email notification.
> NIDS cannot be prevent or stop a breach or attack against on its own.
> It receive copy of all traffic and evaluates it against a set of standards:
 1. Signature Based: 
  - Evaluated network traffic for known malware or attack signatures.
 2. Anomaly Based: 
  - Evaluate network traffic for suspicious changes.
 3. Policy Based:
  - Evaluate network traffic against a specific declared security policy
 4. heuristic Based:
  - Evaluate network traffic against past network behaviour (look for expected pattern changes)
> May be deployed at the host level:
 1. Host-based Intrusion Detection System (HIDS)

### Network-based Intrusion Prevention System (NIPS)
> NIPS is an active system designed stop a breach or attack from succeeding in damaging the network:
 1. Perform an action or set of actions to stop the malicious activity.
 2. Will inform the network administrator through the use of log files, SMS, and email notification.
> All traffic will go though the NIPS to either enter or leave the segment:
 1. All traffic is evaluated against a set of standards.
> Placement of NIPS is on between a router (with a firewall) and the destination network segment.
> NIPS will be active on response of situation:
 1. Block the offending IP address.
 2. Close the vulnerable interface.
 3. Terminate the network session.
 4. Redirect the attack.
 5. Perform additional actions.
 
###	UNIFIED Threat Management (UTM) Security Appliance
 > All possible all in one security solution:
 1. Contains firewall features.
 2. Contains IDS features.
 3. Contains antivirus and antimalware features.
 4. Contains anti-spam features.
 5. Can perform content and URL (Web) filtering.
 6. Can also perform additional functions.
> In a form of a network appliance.
 1. Special designed piece of hardware with an integrated software package-creating a closed system.
> Pros:
 1. Provide multiple security features in a central location.
 2. Simplifies management of security.
 3. Eases updating security.
> Cons:
 1. Concentrates security in a single system or location.
 2. This can create a single point of failure for both the network and for security.

# INTRODUCTION TO NETWORK DEVICES [PART 3]
- Spam Filter.
- Network Devices.

## spam Filter
### Spam Define:
> Defined as unsolicited bulk email (UBE), or junk email.
> The spammer is hoping that the recipient will buy a product or service:
 1. Most cases receive of spam is not a security threat, but it considered a waste of resources.
 
### Filter for spam:
> it usually put on the SMTP server to reduce the amount of spam that is received.
1. Real-time blacklist (RBL): 
- A subscription services that provides a list of known IP address of spam hosts, which than allow them to be blocked.
2.Connection Filter:
Prohibiting a list of specific IP addresses from connecting to a SMPT server.
3. Recipient Filter:
- Blocking messages sent from a particular recipient.
4. Sender Filter:
- Blocking messages sent form particular entity.
5. Sender ID Filter:
- Allow an SMTP server to review the sender policy framework (SPF) record of the sender in DNS. If the sending SMTP server is listed then the messages is accepted

### History Of SPAM:
> Occur in 1978 which involved an advertisement for Digital Equipment Corporation (DEC) computers
> While the reaction for UBE is negative, but it did some sales.
> The term is known as UBE. Because of Monty Python’s flying Circus for the term SPAM in 1970. This effectively may block the useful information

## Network Devices 
### Web Security Gateway:
> A system designed to protect network from malicious content that is on the internet.
1. It can be used to filter prohibited content.
2. It can be used to scan for malicious code.

> These can also be use as a data loss prevention (DLP) measure:
 1. Outgoing content is scanned. If sensitive content is discovered in the scan, It is not allowed to leave the network
 
### Protocol analyzer:
> Often called as packet sniffer.

> Examines the network behaviour at very basic level; they allow for the examination of the individual packets of data.

> Can be used to see what consuming network resources is (e.g., is something going bad with the interface).

> Can be use to identify network breach or attack.

> Can be used to study the method used to create the network breach.

> Tools:
1. Wireshark.
### Web Application Firewall:
> Is an application layer (Layer 7) firewall that is used to control HTTP traffic that can reach the webserver.

> This allow greater inspection and control of messages and traffic that is destined to a network’s Web Servers.

> This can control and protect the servers from common attack.

> Web application Firewall is different from normal network firewall:
1. Web application Firewall protect what is attempting to the web server.
2. Network Firewall protect the network as a whole.

## integrating Data and System with third parties 
- Evaluate the risks of integration.
- Considerations of integration.

## Evaluate the risks of integration
> The key is to know the risk
 
> System and data may be required to integrated because of joint venture with another entity. When implementing the cloud computing, there will be needed to integrate systems and data.

> The need is well known intentional, while the other case it may not recognized as happening. When people use social media, the may actually integrate the company data with third party.

> In all case, there is a risk within the integration data with third parties.

# Considerations of integration [PART 4]
### Risk awareness:
1. Always evaluate the risk when integrating system and data with third parties:
- Data may reside out of control of the business.
- Network transmission may be vulnerable.
- The other side of integration may not be secure.
- The party may go out of business.

### Onboarding and offboarding of business partners.
1.  THE ONBOARDING PROCESS: Procedures and systems need to be put in place that will allow authorized people from the third-party business partner to access the appropriate system and data.
- Implementing an identify and access management (IAM) system can help ease the burden.
2. THE OFFBOARDING PROCESS: Procedures and systems also need to be put in place to remove access once the partnership is terminated or the authorized person leaves the business partner.

### Interoperability agreements.
1. If the integration of the risk is acceptable, some of additional agreement need to be created to help the process:
- MEMORANDUM OF UNDERSTANDING (MOU): A document that is created that established an agreement between two parties.
- BLANKET PURCHASE AGREEMENT (BPA): A document created and used for covering repetitive needs for products or services.
- SERVICE LEVEL AGREEMENT (SLA): An agreement that specifies the guaranteed uptime of the system.
- INTERNET SERVICE AGREEMENT (ISA): Specifies any data limits places on an internet connection and should contain a guarantee of the amount of uptime of the internet connection.

### Data Backups.
1. Cloud storage may be the best solution to off site storage for the data backups-mitigating the risk of data loss in case of a disaster.
- A risk associated with the third party; All backups store offsite should be encrypted.
 
### Data ownership.
1. There must be clear understanding of data ownership before integration of system and data is undertaken.
- Some third parties consider all data stored on their systems as being their data.

### Compliance and Performance Standard.
1. Real all the agreements with third parties carefully to ensure that what they offer an/or provide meets with the compliance standards that are required.
- In some cases, it is not only inappropriate to integrate data with a third party, but it may also actually be in violation of the law.

### Follow security policies and procedures.
1. Security policies and procedures should be in place to protect the integrity of the business’s system.
- At least one of the policies needs to define what is unauthorized sharing of data.

### Social media represents a type of data integration that may be difficult to control.
1. With the increase on social media network and application, company data may not necessarily be under control of the proper entities.
2. Companies should strive to train personnel on what appropriate to share on social media and what should not. 
3. It is possible that company sensitive information may be shared on social media.

# Type of Application Attack 1 [PART5]
- Application attacks defined.
- Common application attacks.
> Due to improvement in modern network security, it may not be easy to exploit the network resources.

> As the improvement in modern network security, attackers have shifted their focus to application attacks. The hacker will focus on exploiting weakness in the software and operating systems that people use every day.

> A poorly developed application can often give the hacker an access to system if the exploit executed perfectly.

## Cross-Site Scripting (XSS) Attack.

- The hacker inserts script code into a form on a web page that get submitted to the server:
1. The server submit the script code to another client system, which then executes the script.
- XSS often used to attack database servers that are used to support web pages.

## Structured Query Language (SQL) injection attack.

- SQL is the common language used to manipulate databases. Most business and web app use SQL to retrieve data from databases.
- To perform attack, hacker insert SQL commands to application, usually from an input field, knowing that the application will pass the command to the database application:
1. The injected SQL commands will then modify the database such as inserting new username and password, so that will enable access to hacker to exploit.

## Buffer Overflow Attack.

- Hacker sends more information to the application than the application’s memory buffer can handle.
1. The additional information will often be placed in memory outside the buffer.
2. If the hacker can get the right information stored outside of the buffer, hacker can execute code with administrative privilege.
-For example, an attacker may introduce extra code, sending new instructions to the application to gain access to IT systems.
-If attackers know the memory layout of a program, they can intentionally feed input that the buffer cannot store, and overwrite areas that hold executable code, replacing it with their own code. For example, an attacker can overwrite a pointer (an object that points to another area in memory) and point it to an exploit payload, to gain control over the program.

## Integer Overflow Attack.

- Like buffer overflow but exploit with mathematical function of an application.
1. When a mathematical function returns an integer larger than the memory space that has been allocated to receive it, application often respond in unexpected ways; This represents a security issue.  

## Directory Traversal/Command Injection Attack.

- Attack against server which hacker attempts to traverse the web server’s directories where the hacker can execute command on the web server OS:
1. Hacker manipulate the URL request in order to get into directories and get a command prompt on the undelaying OS.

## LDAP (Lightweight Directory Access Protocol) injection attack.

- Uses same principle as an SQL injection attack, but exploits LDAP calls instead of SQL commands.

## XML (Extensible Markup Language) Injection attack.

- Uses same principle as the SQL and LDAP attacks, but exploit XMP to modify the targeted application.

1. One of largest network threat is ZERO DAY ATTACKS. The attack advantage of either new or very recently discovered vulnerabilities in applications, which means that the networks and systems probably have not yet been hardened against them. Security expert must up be willing to adapt to keep pace.
2. The best defence begin with the application’s developer. Most attack against application involve exploiting outside input to the application. By using proper data validation technique, developer can stop most application attack from succeeding.
3. All data validation needs to test through unaffiliated person or organization in order to increase effectiveness of testing.

# Secure Network Administration Concept [Part 6]
- Ruled-based management
- Additional secure network administration concepts.

## Rule Based management field.
- Used to create a secure network environment. Rule-Based management should be designed and tested to ensure that the rule function as expected.

## Firewall rules.
- Should be configured in such a way that only the required traffic can pass through.
1. Whenever possible, the default rule should be denying traffic.
2. Exceptions are then created to allow the required traffic.

- The last rule on any firewall should be an implicit deny statement.
1. Unless explicit allowed, the traffic is denied entry into the network

## Access Control List (ACL).
- Firewall rules often called ACLs.
- Files and folders can have ACLs placed on them using permissions.
- Router can have two ACLs per network interface:
1. One ACL is on the inbound side of interface.
2. The other ACL is on the outbound of the interface.

-   All ACL end with an implicit denies statement.
1. If not explicitly allowed in the ACL, the traffic or request is denied.

- Once created, the ACL should be tested for functionality.
1. To ensure that required action are allowed.
2. To ensure that non-required action is not allowed.

## Additional secure network administration concepts
- Secure router configuration:
1. Put active ACLs in a place. Disable default username and password. Require passwords for all access to the router. Whenever possible, use only secure protocol for access.

- Port Security:
1. Enable security on all switch ports. This limits the ability of an attacker to gain access through a switch. MAC filtering is the security method that is most used.

- Network Separation:
1. Separate and group network resources by function and security needs. This can create more secure areas within a network. Separation can be achieved through VLAN management.

- VLAN management:
1. Change default management VLANs. Proper VLAN management keeps network traffic where it belongs. To allow inter-VLAN communication, the traffic must pass through a router.

- Flood Guards:
1. Most common attack is DOS attack. The attacker floods the network with traffic to block legitimate traffic. Flood guards can recognize the pattern and defend from flood attack.

- Loop protection:
1. Preventing unnecessary network traffic. Redundant routes can create routing loops. Routers use a time-to-live (TTL) value and split horizon to combat this. Redundant links on switches can also creates loops. Spanning Tree Protocol (STP) will negate the loops.

- 802.1x:
1. 802.1x is an authentication protocol used on wireless networks. It requires users to authenticate against a central database before access to the network is granted.

- Unified Management:
1. is a possible all-in-one security solution. UTM system provide multiple security function (firewall and antivirus) ian a single network appliance.

- Log Analysis:
1. Security, system and application logs must reviewed on a regular basis. All to often they are only reviewed when problem has occurred in log files.


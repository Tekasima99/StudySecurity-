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


 


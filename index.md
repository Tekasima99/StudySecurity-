# INTRODUCTION TO NETWORK DEVICES (PART 1)

- Open System Interconnection model
- Basic Network Devices

## Open System Interconnection model:

Was developed way to help disparate computing systems communication with each other.
Security can be place in various layers of OSI model to create a layered security arrangement that will improve the security of an overall performance

OSI LAYER:
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
- Switch.
```markdown
> Utilized as an Application-Specific Integrated Circuit(ASIC) and considered as LAYER 2 OSI device:
 1. ASIC chip has specific programing that allow switch to learn when a device is on the network and which ports it is connected to cia that device's layer 2 MAC address.
> Managed switches allow for security to be placed on inviduals switch ports and creating more secure enviroment in networking
> Switch only communicate with local network devices.
```
- Wireless Access Point(WAP).
```markdown
> WAP is a specific type of network that connect wireless network segments with wired network segments and considered as as layer 2 OSI device:
  1. Wireless network segments WAP bridges (802.11)
  2. Ethernet network segments (802.3)
> WAP are capable to utilizing encyrption to help esure a secure network networking enviroment.
> WAP only communicate with local network devices
```
- Multilayer Switch (MLS).
```markdown
> MLS provides normal layer 2 network switching services, but also provide layer 3 or higher OSI model services.
> Most common MLS is a layer 3 switch.
> MLS commonly implements security at layer 2 and higher on OSI model.
```
- Router.
```markdown
> Most common network device for connecting different network together utilizing the layer 3 OSI model logical network information.
> Router uses software programming for decision making, as compared to the switches use of an ASIC chip.
> Firewall and ACL usually placed on router to help secure networks
```
- Firewall.
```markdown
> Can be placed on router or host (software based) or  can be its own device(network appliance)
> It function on multiple layer of OSI model layer(2,3,4,7).
> Block packet from entering and leaving the network:
 1. Stateless Inspection, which examine every packet that against a set of rule. When packet matches a rule, the rule is enforced and the specified action is taken.
 2. Stateful Inspection, which the firewall only examine the state of the connection between networks specially when a connection is made from an internal network to an external network, the firewall will not examine any packets running from the external connection. As a general rule, external connetion not allowed to be initiated with the internal network.
> First line of defense.
```
- Load Balancer.
```markdown
> May also be called a content switch or content filter:
 1. Can be implemented to increase the security of the network by limiting or filtering the content that is allowed.
> A network appliance taht used to load balance between multiple hosts that contain the same data spreading out the workload for greater efficiency.
 1. Used to distribute the requests(workload) to a server farm among the various servers that help no single server gets overload.
```
- Proxy Server.
```markdown
> Is an appliance that requests resources on behalf of client machines.
> Often used to retrieve resources from untrusted ousider network on behalf of the requesting client.
> It hides and protects the requesting client.
> Can be utilized to filter allowed content.
> Can be increase performance by caching commonly requested web pages.
```
 
 
 


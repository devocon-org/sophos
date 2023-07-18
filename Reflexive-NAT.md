## Reflexive NAT for Sophos firewall 

Reflexive NAT: 

* Reflexive NAT, also known as NAT with stateful packet inspection (SPI), is a type of NAT that dynamically maps internal IP addresses and ports to external IP addresses and ports. 
It is commonly used to allow internal hosts to initiate outbound connections to the Internet, while maintaining state information to allow inbound traffic to return to the correct internal host.

* When an internal host sends an outbound packet through a firewall with reflexive NAT enabled, the firewall creates a temporary mapping in its NAT table to track the internal IP address, internal port, external IP address, and external port. This mapping allows the firewall to correctly route incoming responses back to the internal host that initiated the connection.

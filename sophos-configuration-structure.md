## sophos-configuration-structure.md

An IP address is a numerical label assigned to the devices connected to a computer network that uses the IP for communication. IP address act as an identifier for a specific machine on a particular network. It also helps you to develop a virtual connection between a destination and a source.

_**Types of Website IP Addresses**_

* Share IP Address
* Dedicated IP Address

_**Shared IP Addresses**_

Shared IP address is used by small business websites that do not yet get many visitors or have many files or pages on their site. The IP address is not unique and it is shared with other websites.

_**Dedicated IP Addresses**_

Dedicated IP address is assigned uniquely to each website. Dedicated IP addresses helps you avoid any potential backlists because of bad behavior from others on your server. The dedicated IP address also gives you the option of pulling up your website using the IP address alone, instead of your domain name. It also helps you to access your website when you are waiting on a domain transfer.

_**Version of IP address**_

 * IPV4
 * IPV6.

**IPV4**

IPv4 was the first version of IP. It was deployed for production in the ARPANET in 1983. Today it is the most widely used IP version. It is used to identify devices on a network using an addressing system.

The IPv4 uses a 32-bit address scheme allowing to store 2^32 addresses, which is more than 4 billion addresses. To date, it is considered the primary Internet Protocol and carries 94% of Internet traffic.

**IPV6**

It is the most recent version of the Internet Protocol. Internet Engineer Taskforce initiated it in early 1994. The design and development of that suite is now called IPv6.

This new IP address version is being deployed to fulfill the need for more Internet addresses. It was aimed to resolve issues which are associated with IPv4. With 128-bit address space, it allows 340 undecillion unique address space.

**IP Address Classification Based on Operational Characteristics**

_**Unicast addressing**_

Unicast addressing is the most common concept of an IP address in the Unicast addressing method. It is available in both IPv4 and IPv6.

This IP address method refers to a single sender/receiver. It can be used for both sending and receiving the data.

In most cases, a Unicast address is associated with a single device or host, but a device or host that may have more than one unicast address.

_**Broadcast addressing**_

Broadcasting addressing is another addressing method available in IPv4. It allows you to manage data to all destinations on a network with a single transmission operation.

The IP address 255.255.255.255 is mostly used for network broadcast. Moreover, limited directed-broadcast uses the all-ones host address with the network prefix.

IPv6 does not provide any implementation and any broadcast addressing. It replaces it with multicast to the specially defined all-nodes of the multicast address.

_**Multicast IP addresses**_

Multicast IP addresses are used mainly for one-to-many communication. Multicast messages are mostly sent to the IP multicast group address.

In this, routers forward copies of the packet out to every interface with hosts subscribed to that specific group address. Only the hosts that require receiving the message will process the packets. All other hosts on that LAN will discard them.

_**Anycast addressing**_

In anycast addressing the data, the stream is not transmitted to all receivers. However, just the one that the router decides is closest to the network.

This IP addressing comes as a built-in feature of IPv6. In IPv4, it is implemented by using the Border Gateway Protocol by using the shortest-path metric. This method is widely used for global load balancing and is also used in distributed DNS systems.

_**IP Classification**_

|CLASS|START RANGE|END RANGE|PRIVATE IPS| LEADING BITS|
|---|---|---|----|---|
|A|1|127|10.0.0.0      - 10.255.255.255| /8 |
|B|128|191|171.16.0.0  - 172.31.0.0| /16 |
|C|192|223|192.168.0.0 - 192.168.255.255| /24 |

**Private IPv4 addresses details**

|RFC 1918 name|	IP address range	|Number of addresses	| Largest CIDR block (subnet mask)|	Host ID size	|Mask bits	Classful description|
|---|---|---|---|---|---|
|24-bit block	|10.0.0.0 – 10.255.255.255	|16777216|10.0.0.0/8 (255.0.0.0)|	24 bits	|8 bits|	single class A network|
|20-bit block	|172.16.0.0 – 172.31.255.255|	1048576	|172.16.0.0/12 (255.240.0.0)|	20 bits|	12 bits	| 16 contiguous class B networks|
|16-bit block	|192.168.0.0 – 192.168.255.255|65536|192.168.0.0/16 (255.255.0.0)|	16 bits	|16 bits	|256 contiguous class C networks|

_**Private Class A case study**_

In this case, we'll assume the five regions and their user information. We have a different firewall and details depending on the region.

_**Planning of multiple firewall configuration**_

| LOCATION | USERS  | NETWORKS   | IP ADDRESSES |  ACTUAL HOSTS | GATEWAY |
|---|---|---|---|---|---|
| DEL | 300 | 10.1.10.0/23 | 10.1.10.1 - 10.1.11.254 | 512 - 2  | 10.1.10.1 |
| CHE | 100| 10.1.12.0/25  | 10.1.12.1 - 10.1.12.126 | 128 - 2  | 10.1.12.1 | 
| MUM | 210 | 10.1.13.0/24 | 10.1.13.1 - 10.1.13.254 | 256 - 2  | 10.1.13.1 |
| BAN | 300 | 10.1.14.0/23 | 10.1.14.1 - 10.1.15.254 | 512 - 2  | 10.1.14.1 |
| KOC | 700 | 10.1.16.0/22 | 10.1.16.1 - 10.1.19.254 | 1024 - 2 | 10.1.16.1 |

_**Private Class B case study**_



## creating ssl vpn group rule for firewall


|_Source_|_Source Network_|
|---|---|
|VPN|VPN-IP-Ranges|


|_Destination_|_Destination-Network_|ports|
|---|---|---|
|LAN|Server-ip address|port-numb|


**_First create SSL_VPN(remote-acccess) config in `VPN`_**

* Under Identity Edit Policy members add users or group u want to give remote access

* Under Tunnel access edit Permitted network resources (IPv4), add all the internal server's ip add u want users to access

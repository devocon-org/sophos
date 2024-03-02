## New-sophos-firewall-configuraton.md

_**Default Console Login**_

|username|password|address|port|
|---|---|---|---|
|admin|admin|172.16.16.16|4444

open your browser _https://172.16.16.16:4444_


![image](https://user-images.githubusercontent.com/102893121/174487952-4f977ff2-d2de-47d0-859f-8a7a52c3abc3.png)



After logging in to the console Look at the left side column. To select **Network** 

![1](https://user-images.githubusercontent.com/102893121/174487653-2ca89554-491b-4cda-a2ee-5e2775ec4a2b.png)


Inside the DHCP Section, check the status of the Default DHCP Server and disable it.

![2](https://user-images.githubusercontent.com/102893121/174487690-da787824-e905-4599-9c94-3cd020d4d6cc.png)

Once you disable the DHCP server, Go to the Interface Section and select `br0`

![3](https://user-images.githubusercontent.com/102893121/174487752-7d145622-a771-432d-af0c-fff083c7dc5a.png)

After enter the br0 change the `IP4` and `Netmask` and Save 

| IP | SubnetMask |
|---|---|
|10.5.0.1|24/255.255.255.0|


![image](https://user-images.githubusercontent.com/102893121/174487758-1108dab7-ffbd-4a02-a0f7-3d0ec0291b19.png)

Above the Process Don, then manually assigned Ip in your Local machine 

Follow the process

setting > network > wired setting > IPV4 tab > change Automatic to Manual > (Your changed IP) (subnetmask) and (gateway) > save > restart your wired setting(Click OFF and ON)


After manually Assign the IP

Login with your Changed IP in that case I will change `10.5.0.1` so i will use https://10.5.0.1:4444 

Then GO to Network then change the DHCP tab and click the `Default DHCP server` setting and set your Ip range and save then enable your DHCP.

![image](https://user-images.githubusercontent.com/102893121/174487766-0cd5d901-81db-4fc2-96d9-50d94baf635d.png)

then enable your Default DHCP. and change your local machine DHCP config

setting > network > wired setting > IPV4 tab > change Manual to Automatic 

![image](https://user-images.githubusercontent.com/102893121/174487777-8bb7324a-d6f9-4221-85e5-faa54602280d.png)

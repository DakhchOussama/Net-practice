Address ip : An IP address is a unique address that identifies a device(machine) on the internet or a local network. IP stands for "Internet Protocol," which is the set of rules governing the format of data sent via the internet or local network.

In essence, IP addresses are the identifier that allows information to be sent between devices on a network: they contain location information and make devices accessible for communication. The internet needs a way to differentiate between different computers, routers, and websites. IP addresses provide a way of doing so and form an essential part of how the internet works.

An IP address is a string of numbers separated by periods. IP addresses are expressed as a set of four numbers — an example address might be 192.158.1.38. Each number in the set can range from 0 to 255. So, the full IP addressing range goes from 0.0.0.0 to 255.255.255.255

The use of IP addresses typically happens behind the scenes. The process works like this:

1. Your device indirectly connects to the internet by connecting at first to a network connected to the internet, which then grants your device access to the internet.
2. When you are ~~at~~ home, that network will probably be your Internet Service Provider (ISP). At work, it will be your company network.
3. Your IP address is assigned to your device by your ISP.
4. Your internet activity goes through the ISP, and they route it back to you, using your IP address. Since they are giving you access to the internet, it is their role to assign an IP address to your device.
5. However, your IP address can change. For example, turning your modem or router on or off can change it. Or you can contact your ISP, and they can change it for you.
6. When you are out and about – for example, traveling – and you take your device with you, your home IP address does not come with you. This is because you will be using another network (Wi-Fi at a hotel, airport, or coffee shop, etc.) to access the internet and will be using a different (and temporary) IP address, assigned to you by the ISP of the hotel, airport or coffee shop.

![isp-internet-service-provider-definition.jpeg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1f32833e-7ebd-4c1f-a163-744a32766c7b/isp-internet-service-provider-definition.jpeg)

**Adresse IP** :

octet1 . octet2 . octet3. octet4

1 octet = 8 bits

xxxxxxxx . xxxxxxxx . xxxxxxxx . xxxxxxxx

bit = binary digit

x ⇒ {0, 1}

10000000 . 00001010 . 11011000 . 0010011

to decimal ⇒ 128 . 10 . 216 . 39

**Valeur max** ⇒ 0000 0000 = 0 | 1111 1111 = 255

**Les classes :** 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/19f5962c-308d-48da-b49b-025320b77ec1/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5e596a62-6fe7-488c-a983-07e76ca9af8e/Untitled.png)

Class A ⇒ started from 0.0.0.0 to 127.255.255.255

Class B ⇒ started from 128.0.0.0 to 191.255.255.255

Class C ⇒ started from 192.0.0.0 to 223.255.255.255

Class D ⇒ started from 224.0.0.0 to 239.255.255.255

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c8dea6ca-7d08-44e1-8eda-975383715159/Untitled.png)

Green Part ⇒ HOTE Part

Grey Part ⇒ Reseau Part

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b0b069b0-229d-4c77-995b-a29ef7c55972/Untitled.png)

how many hotes we have ⇒ 2 us n - 2

how many reseau we have ⇒ 2 us n

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a40d2ce1-63b3-4722-91e2-104ba9522143/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7a6c744c-1bc0-4248-a159-314af3a7cd28/Untitled.png)

# **Network Masking**

The network mask is used to determine which portion of the IP address is the network address and which is the host address. This means that the portions of network to host in an IP address can change. The most common network mask is 255.255.255.0. The simple explanation is that wherever there is a 255, this indicates that it is the network portion. Wherever there is a 0, this indicates the host portion (part).

ip add 192.168.100.2 and subnet mask 255.255.255.0 now 192.168.100.X is network id which is used to identify from which network u belongs to and x is host id which is unique for every node on network

Think of it as the street name vs the street address. Say you live at 123 S. Elm St. The street is S. Elm St. Your address is 123 ON S. Elm St.

When you have an IP address of 10.0.1.135 with a mask of 255.255.255.0, that means that your **network** is 10.0.1.0. That’s the street. Your **host** address is #135 on 10.0.1.0 street.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1e802d93-a4aa-4780-b11b-f1a9eb0c88ef/Untitled.png)

Subnet Mask : /30 ⇒ how many num 1 we have 11111111.1111111.11111111.11111100

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/64776607-e495-4fb5-8b5c-30cfade71b74/Untitled.png)

A subnet mask is a 32 bits (4 bytes) address used to distinguish between a network address and a host address in the IP address. It defines the range of IP addresses that can be used within a network or a subnet.

****Finding the network address****

To determine which portion of the IP address is the network address, we need to apply the mask to the IP address. Let's first convert the mask to its binary form:

`Mask | 11111111.11111111.11111111.10000000`

The bits of a mask that are 1 represent the network address, while the remaining bits of a mask that are 0 represent the host address.

More information : https://github.com/lpaube/NetPractice

****the network address vs host addresses ????????????****

# Switch :

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b5affe48-d754-4629-b0f8-7b7b6765b220/Untitled.png)

A switch connects multiple devices together in a single network. Unlike a router, the switch does not have any interfaces since it only distibutes packets to its local network, and cannot talk directly to a network outside of its own.

# Router :

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/69f00b0f-2625-4ac3-b056-c5b1ff615cee/Untitled.png)

Just as the switch connects multiple devices on a single network, the router connects multiple networks together. The router has an interface for each network it connects to.

Since the router separates different networks, the range of possible IP addresses on one of its interface must not overlap with the range of its other interfaces. An overlap in the IP address range would imply that the interfaces are on the same network.

****Routing Table :****

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/22b604a2-dc7c-4cff-80a9-816d2ff9009b/Untitled.png)

![Screen Shot 2022-07-26 at 9.32.08 PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/15094ff5-1558-415e-9fc7-41a43a783f21/Screen_Shot_2022-07-26_at_9.32.08_PM.png)

### **Public Address vs. Private Address**

A public IP address is an IP address that can be accessed directly over the internet and is assigned to your network router by your internet service provider (ISP). A public (or external) IP address helps you connect to the internet from inside your network, to outside your network.

A private IP address is the address your network router assigns to your device. Each device within the same network is assigned a unique private IP address (sometimes called a private network address) — this is how devices on the same internal network talk to each other.

When a network is connected to the internet, it cannot use an IP address from the reserved private IP addresses. The following ranges are reserved for private IP addresses:

192.168.0.0 – 192.168.255.255 (65,536 IP addresses)
172.16.0.0 – 172.31.255.255   (1,048,576 IP addresses)
10.0.0.0 – 10.255.255.255     (16,777,216 IP addresses)

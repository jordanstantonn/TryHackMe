# Cisco Packet Tracer Lab – Home Network Configuration

## Network Topology Setup

I began by adding the required devices to the Packet Tracer workspace, including a PC, a laptop, a wireless router, a cable modem, and the Internet cloud. Once the devices were in place, I connected them using the appropriate cabling. The PC was connected to the wireless router with a copper straight-through cable, the wireless router was connected to the cable modem with a copper crossover cable, and the cable modem was connected to the Internet cloud using a coaxial cable.


## PC Configuration

After building the topology, I verified that the PC was configured to obtain its network settings automatically through DHCP by checking **Desktop → IP Configuration**. Since the PC was already set to use DHCP, it automatically received its network configuration.

<img width="1027" height="999" alt="image" src="https://github.com/user-attachments/assets/24eab081-af8f-4146-a3b9-42cd42d64118" />


To confirm that the configuration was successful, I opened the Command Prompt and ran:

```text
ipconfig /all
```

The output showed that the PC had successfully obtained an IP address, subnet mask, default gateway, and DNS server from the DHCP server.

## Connectivity Verification

With the PC configured, I tested network connectivity by running:

```text
ping cisco.srv
```

The successful replies confirmed that the PC could communicate with the Cisco server and that the network was functioning as expected.
<img width="1038" height="826" alt="image" src="https://github.com/user-attachments/assets/fa716e2d-95fa-4e97-870c-873b5c77ab74" />

## Laptop Wireless Configuration

Next, I configured the laptop for wireless connectivity. Since the laptop initially contained a wired Ethernet module, I replaced it with the **Wireless WPC300N** module through the Physical tab. After powering the laptop back on, I opened **PC Wireless**, located the **HomeNetwork** wireless network, and connected to it.

Once connected, I verified that the laptop had successfully joined the wireless network by pinging **cisco.srv**. The successful responses confirmed that both the wired and wireless devices had network connectivity.

## Results

By the end of the lab, both the PC and laptop successfully obtained IP addresses through DHCP and were able to communicate with the Cisco server. This lab reinforced the process of creating a basic home network topology, verifying DHCP configuration, testing connectivity, and configuring a wireless client in Cisco Packet Tracer.

## Final IP Addressing

The final IP addressing table is shown below.

*Insert screenshot of the completed IP addressing table here.*

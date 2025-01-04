# Cisco Networking Basics: Creating a LAN - Packet Tracer

## Overview
This project demonstrates the setup of a Local Area Network (LAN) using Cisco Packet Tracer. A LAN is a collection of devices connected in a single physical location, such as a building, office, or home. LANs can range from small home networks with a single user to enterprise networks with thousands of users and devices.

### Objectives
1. Connect network devices and hosts.
2. Configure devices with IPv4 addressing.
3. Verify the end device configuration and connectivity.
4. Use networking commands to view host information.

### Resources
- **Video demonstration**: [YouTube Link](https://www.youtube.com/watch?v=jOmqFi28hDI&list=PLC0b3C1jAAo4DxLxsaXrt0SLeLSFQq-t-&index=2)
- **Screenshots**: Included per objective for better understanding.

---

## Addressing Table
| Device         | Interface/Port | IPv4 Address      | Subnet Mask      |
|----------------|----------------|-------------------|------------------|
| Admin PC       | NIC            | DHCP              | N/A              |
| Manager PC     | NIC            | DHCP              | N/A              |
| Printer        | NIC            | 192.168.1.100     | 255.255.255.0    |
| www.cisco.pt   | NIC            | 209.165.200.225   | N/A              |

---

## Instructions

### Part 1: Connect Network Devices and Hosts

#### Step 1: Power on Devices
- Open the **Physical Tab** for each device.
- Turn on the power switch in the **Physical Device View** window.
- Verify that the green power light is illuminated.

#### Step 2: Connect Devices
Use the following connection table to set up the network:

| Device        | Interface/Port  | Connected Device  | Connection Interface/Port |
|---------------|-----------------|-------------------|---------------------------|
| Office Router | G0/0            | ISP1             | G0/0                      |
| Office Router | G0/1            | Switch           | G0/1                      |
| Admin PC      | NIC (F/0)       | Switch           | F0/1                      |
| Manager PC    | NIC (F/0)       | Switch           | F0/2                      |
| Printer       | NIC (F/0)       | Switch           | F0/24                     |

- Use Ethernet copper straight-through cables for all connections.
- Verify green link lights on all connections.

---

### Part 2: Configure Devices with IPv4 Addressing

#### Step 1: Configure Hosts
- **Admin PC and Manager PC**:
  - Set to receive IP addresses dynamically from DHCP.
  - Use the **Desktop > IP Configuration** application.
- **Printer**:
  - Configure manually with the static IP address from the Addressing Table.
  - Open the **Config tab > FastEthernet0 interface** and input the IP address and subnet mask.

---

### Part 3: Verify the End Device Configuration and Connectivity

#### Step 1: Verify PC Connectivity
- Check IP addressing configuration from the desktops of the PCs.
- Use **ping** to test connectivity with the Printer from Admin PC and Manager PC.
  - Example: `ping 192.168.1.100`

#### Step 2: Verify Internet Connectivity
- Open the Web Browser on the PCs.
- Access the internet server using its IP address and URL.
  - Example: IP address: `209.165.200.225`; URL: `www.cisco.pt`.

---

### Part 4: Use Networking Commands to View Host Information

#### Step 1: Use the `ipconfig` Command
- Open Command Prompt on a PC.
- Run `ipconfig` and `ipconfig /all`.
- Note the additional details provided by `ipconfig /all`.

#### Step 2: Use the `tracert` Command
- From a PC, use `tracert` to trace the route to the web server’s URL.
  - Example: `tracert www.cisco.pt`.

---

## Conclusion
This project demonstrated the basic setup of a LAN using Packet Tracer. By following these steps, you learned how to connect devices, configure IPv4 addressing, verify connectivity, and use networking commands to gather host information. Refer to the [YouTube demonstration](#) and screenshots for further guidance.


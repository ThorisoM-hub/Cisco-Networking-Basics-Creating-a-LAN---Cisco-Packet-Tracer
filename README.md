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

![Power on Devices](file-TVW7fw9AohHwCA2BEcjQ8w)

#### Step 2: Connect Devices
Use the following connection table to set up the network:

| Device        | Interface/Port  | Connected Device  | Connection Interface/Port |
|---------------|-----------------|-------------------|---------------------------|
| Office Router | G0/0            | ISP1             | G0/0                      |
| Office Router | G0/1            | Switch           | G0/1                      |
| Admin PC      | NIC (F/0)       | Switch           | F0/1                      |
| Manager PC    | NIC (F/0)       | Switch           | F0/2                      |
| Printer       | NIC (F/0)       | Switch           | F0/24                     |

- Use **Ethernet copper straight-through cables** for all connections.
- Verify green link lights on all connections.

![Connection Setup](path-to-your-connection-setup-image.png)

---

### Part 2: Configure Devices with IPv4 Addressing

#### Step 1: Configure Hosts
- **Admin PC and Manager PC**:
  - Set to receive IP addresses dynamically from DHCP.
  - Use the **Desktop > IP Configuration** application.
- **Printer**:
  - Configure manually with the static IP address from the Addressing Table.
  - Open the **Config Tab > FastEthernet0 interface** and input the IP address and subnet mask.

![Configure Admin PC](path-to-admin-pc-ip-configuration-image.png)
![Configure Printer](path-to-printer-ip-configuration-image.png)

---

### Part 3: Verify the End Device Configuration and Connectivity

#### Step 1: Verify PC Connectivity
- Check IP addressing configuration from the desktops of the PCs.
- Use **ping** to test connectivity with the Printer from Admin PC and Manager PC.
  - Example: `ping 192.168.1.100`

![Ping Test Result](path-to-ping-test-result-image.png)

#### Step 2: Verify Internet Connectivity
- Open the **Web Browser** on the PCs.
- Access the internet server using its IP address and URL.
  - Example: IP address: `209.165.200.225`; URL: `www.cisco.pt`.

![Internet Connectivity Test](path-to-internet-connectivity-test-image.png)

---

### Part 4: Use Networking Commands to View Host Information

#### Step 1: Use the `ipconfig` Command
- Open **Command Prompt** on a PC.
- Run `ipconfig` and `ipconfig /all` to display network configuration details.

![IPConfig Output](path-to-ipconfig-output-image.png)

#### Step 2: Use the `tracert` Command
- From a PC, run `tracert www.cisco.pt` to trace the route to the web server's URL.

![Tracert Output](path-to-tracert-output-image.png)

---

### Part 5: Final LAN Diagram with IP Addressing

- **Final Completed Diagram with IP Addressing**: Below is the diagram of the fully completed LAN, showing all the network devices, connections, and **IP configurations**.

   ![LAN Final Diagram](path-to-your-lan-final-diagram.png)

   **IP Addressing Details:**
   - **Admin PC**: DHCP assigned.
   - **Manager PC**: DHCP assigned.
   - **Printer**: Static IP `192.168.1.100`, Subnet Mask `255.255.255.0`.
   - **www.cisco.pt**: Static IP `209.165.200.225`.

---

### Part 6: Show Results of Work

#### Step 1: Capture Screenshots of Results

1. **Connection Test**:
   - Test the network connectivity between devices (e.g., ping or use the email simulation in Packet Tracer to verify connectivity).
   - Capture the **status message** confirming the connection was successful.

   *Example Screenshot:*
   ![Connection Test Result](path-to-your-connection-test-screenshot.png)

2. **Project Requirements: All Answers Correct**:
   - Capture a screenshot showing that all project requirements (such as network setup, IP configuration, and connectivity tests) have been completed successfully, and all answers were marked correct.

   *Example Screenshot (Project Results)**:
   ![All Answers Correct](path-to-your-final-results-screenshot.png)

---

## Conclusion
This project demonstrated the basic setup of a LAN using Packet Tracer. By following these steps, you successfully connected devices, configured IPv4 addressing, verified connectivity, and tested network performance with the connection tests. The screenshots provided above showcase the results of your work, confirming the successful setup and testing of the network.










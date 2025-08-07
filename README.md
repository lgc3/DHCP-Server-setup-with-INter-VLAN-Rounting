# DHCP Server setup with Inter-VLAN Routing <br>
<img width="528" height="272" alt="image" src="https://github.com/user-attachments/assets/8984fea9-7aca-4cf3-9ee1-15d512b2891d" /> <br>


# Technology Utilized
- CISCO Packet Tracer
- Switches
- Routers
- Servers
- VLANs

## Objectives: 
Create a DHCP configuration so that devices in a network can automatically
obtain IP addresses and other network configuration details from a DHCP server.


### Activity 1: Set up the environment by adding Devices to the Workspace
- From the End Devices section and the Network Devices section, drag and drop:
  - PCs for each VLAN/subnet, and add a Server to configure as the DHCP server.
  - ARouter (2911) and  a Switch (2960).
-  Physically Connect Devices
  - Connect the following devices using the copper straight-through cable
    - Router (GigabitEthernet 0/0) to the Switch (FastEthernet 0/24).
    - Each PC to the Switch (FastEthernet 0/1-5 for vlan 10, FastEthernet 0/6-10 for vlan 20, FastEthernet 0/11-15 for vlan 30).
    - The Server (FastEthernet 0) to the Switch (FastEthernet 0/24). <br>
<img width="619" height="369" alt="image" src="https://github.com/user-attachments/assets/4ff5acf2-a7a5-49b7-8ac5-d109cb0f2e35" /> <br>

### Activity 2: Configure the VLANs on the Switch
- Create VLANs:
- Assign PC ports to respective VLANs
- Configure the port connected to the router as a trunk port: <br>
<img width="701" height="446" alt="image" src="https://github.com/user-attachments/assets/c3718d85-eb3d-45d7-9614-6da9a8d19a56" />
<img width="350" height="83" alt="image" src="https://github.com/user-attachments/assets/5e6933e4-a38e-49f2-b723-648307898d4a" />
<img width="660" height="179" alt="image" src="https://github.com/user-attachments/assets/83aebf74-e850-4b76-bac7-660e2869afba" /><br>

### Activity 3: Configure the Router for Inter-VLAN Routing
- Configure Sub-Interfaces for Each VLAN:
- Enable the interface: <br>
<img width="842" height="463" alt="image" src="https://github.com/user-attachments/assets/bfb6f4c5-81a5-480a-8b1d-66d98b29736e" /> <br>

### Activity 4: Configure the DHCP Server
- Assign a Static IP and Default Gateway to the Server: <br>
<img width="837" height="362" alt="image" src="https://github.com/user-attachments/assets/78cfd41b-16b8-4479-bd32-443c7c815821" />
<img width="846" height="370" alt="image" src="https://github.com/user-attachments/assets/0159beab-32d0-4fff-b0d6-21aa537d4388" /><br>
- Enable DHCP on the Server and Configure a DHCP pool for each subnet: <br>
<img width="843" height="420" alt="image" src="https://github.com/user-attachments/assets/d556995c-8b43-4c9f-8394-125aef9097ee" />
<img width="844" height="272" alt="image" src="https://github.com/user-attachments/assets/fcfd44bd-3dad-4655-b2a2-526a8bd1bd01" /><br>

### Activity 5: Configure DHCP Relay on the Router
- Configure IP Helper on each VLAN sub-interface: <br>
<img width="503" height="194" alt="image" src="https://github.com/user-attachments/assets/6c5df010-d3e6-4351-8774-1de5524bb598" /> <br>

### Activity 6: Configure PCs to Obtain IP Addresses via DHCP <br>
<img width="848" height="329" alt="image" src="https://github.com/user-attachments/assets/de763070-44e4-43bc-b9b4-764577a088b6" />
<img width="843" height="306" alt="image" src="https://github.com/user-attachments/assets/df6025ba-0da2-431e-a955-8a7722208ec4" />







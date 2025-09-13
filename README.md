# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:13/9/25
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
(Insert screenshot of your Packet Tracer setup here)<br>
________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication(Pinging from 172.16.31.5 to 172.16.31.2)<br>
At 172.16.31.5
<img width="641" height="634" alt="Screenshot 2025-09-13 144537" src="https://github.com/user-attachments/assets/01151593-111c-476e-bdce-8053f09fda34" />
At 172.16.31.2
<img width="627" height="615" alt="Screenshot 2025-09-13 145026" src="https://github.com/user-attachments/assets/151ee15f-075c-4b9e-b009-7395f91af0fa" />

•	PDU details for remote communication(Pinging from 172.16.31.5 to 10.10.10.2)<br>
At 172.16.31.5
<img width="641" height="634" alt="Screenshot 2025-09-13 144537" src="https://github.com/user-attachments/assets/505d5a7f-d7e5-4fb6-b105-b84bcedd06af" />
At 10.10.10.2
<img width="630" height="583" alt="Screenshot 2025-09-13 151814" src="https://github.com/user-attachments/assets/35654015-71ff-485d-babc-313936a8c6a3" />

•	Tables showing MAC/IP changes through each device<br>
Local Communication(From 172.16.31.5 to 172.16.31.2)
<img width="622" height="137" alt="489140310-5e4c28b1-085d-459c-8bbc-f28ff7f63d16" src="https://github.com/user-attachments/assets/35ff5ba1-89ee-4186-a909-ae498b720283" />
Remote Communication(From 172.16.31.5 to 10.10.10.2)
<img width="616" height="187" alt="489140455-6d59484e-2360-4cb5-bd80-2cb70851bd11" src="https://github.com/user-attachments/assets/3192cf0e-510d-4c31-984e-6f4da3b99259" />


________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.


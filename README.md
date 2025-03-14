# Networking-Practical-1
Network Routing and Switching Assessment 1
## Objectives
In this assessment, you will configure the following:
• Best practice configuration and secure management
• VLAN’s and Trunking
• Layer 3 Switching and Inter-VLAN routing
## Part 1: Basic Device Configuration and SSH Management
- Step 1 – Switch configuration
Hint: Leave the configuration of switch passwords and SSH to the end. Configure
switch hostnames and move to step 2. When you have finished everything else come
back to Step 1.
Apply a best practice / basic device configuration to all switches in your topology. Use
the following passwords etc on all devices.
• All device names are listed in the table at the beginning of this document. When
configuring the device hostnames add your student ID to the beginning of each
devices’ name.
Example:
For device S1 if your student number is 12345 the device name will be 12345-S1
• Console password: bsc2con
• Enable password: bsc2enable
• Local username and password:
o Username: bsc2admin
o Password: localadmin
• SSH configuration
o Domain name: bsc2.local
o Modulus (key length): 2048
o Disable Telnet
Do not use any other passwords, only the ones listed above.
Please add any additional configuration you think is necessary as I have not included
all configuration items above that would normally be in a best practice device
configuration.
Configure interface IP addressing on all switches using the information provided in the
table at the beginning of this document.
Step 2 - PC’s and Servers
Using the information supplied in the table at the beginning of this document configure
static IP addresses on all PC’s and servers.
## Part 2: VLAN and Trunking Configuration
Using the details in the table at the beginning of this document configure the required
VLAN’s and Trunk links on all switches.
- Step 1: Configure VLANs
a. Configure VLAN 10 with the name Staff.
b. Configure VLAN 20 with the name Supervisors.
c. Configure VLAN 30 with the name Engineering.
d. Configure VLAN 40 with the name Accounts.
e. Configure VLAN 99 with the name Management&Native.
f. Configure VLAN 999 with the name Unused
- Step 2: Configure active switch ports.
On the active switch ports configure the following:
a. Configure the ports on S1 and S5 as static access ports as follows:
o FastEthernet 0/1 in VLAN 10
o FastEthernet 0/2 in VLAN 20
o FastEthernet 0/3 in VLAN 30
b. Configure the ports on S3 and S6 as static access ports as follows:
o FastEthernet 0/4 in VLAN 40

o FastEthernet 0/5 in VLAN 99
c. Connect all PC’s and Server’s to the correct port on each switch as detailed in the
table.
- Step 3: Configure Trunk Links
Configure the following Trunk links and set VLAN 99 as the native VLAN.
a. S1 G0/1 to MLS1 G0/1
b. S1 Fa0/24 to S2 Fa0/24
c. S1 Fa0/23 to S3 Fa0/23
d. S4 G0/1 to MLS1 G0/2
e. S4 Fa0/24 to S5 Fa0/24
f. S4 Fa0/23 to S6 Fa0/23
- Step 4: Secure unused switch ports.
a. Move all unused switch ports to VLAN 999.
b. Configure all unused switch ports as static access ports.
c. Deactivate all unused switch ports.
## Part 4 – Layer 3 Switching and Inter VLAN routing
Complete all requirements for Layer 3 switching on MLS1 and configure routing between
VLAN’s.
The following tests should be successful.
o Ping from any device on any VLAN to any other device on any VLAN.
o Browse the Web servers from any PC in any VLAN.

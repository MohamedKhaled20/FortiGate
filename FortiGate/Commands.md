
### Session and Diagnostics

- The command ==**`get sys session list`**== is used for **displaying the current contents of the FortiGate's session table** (or connection tracking table).
    
- The command ==**`diagnose sys ha checksum show`**== is used for **displaying the configuration checksums of all members in an HA cluster** to verify they are synchronized.
    
- The command ==**`diagnose sys ha checksum cluster`**== is used for **actively recalculating the configuration checksums for all members of the HA cluster** and displaying the results.
    
- The command ==**`execute ha manage <id> admin`**== is used for **accessing the CLI of a specific member in an HA cluster** directly from the console of another member.
    

### System Configuration (NAT, SD-WAN)

- The command sequence ==**`config system settings`**== then ==**`set central-nat enable`**== is used for **switching the FortiGate from Policy-based NAT to Central NAT mode**.
    
- The command sequence ==**`config system global`**== then ==**`set gui-app-detection-sdwan enable`**== is used for **making the application detection feature visible in the SD-WAN rules GUI**.
    

### Interface Configuration

- The command sequence ==**`config system interface`**==, followed by ==**`edit port8`**==, ==**`set ip 10.0.11.251/24`**==, ==**`set allowaccess ping ssh snmp https`**==, and ==**`end`**== is used for **configuring the firewall's 'port8' interface with a static IP address and defining the allowed administrative access protocols**.
    

### Firewall Policy Configuration

- The command ==**`config firewall policy`**== is used for **entering the configuration mode** for the FortiGate's **firewall policies**.
    
- The command ==**`set inspection-mode proxy`**== is used for **setting the policy's inspection method to 'Proxy-based' instead of the default 'Flow-based'**.
    

### High Availability (HA) Configuration

- The command sequence ==**`config system ha`**==, followed by ==**`set mode a-p`**==, ==**`set group-name Training`**==, ==**`set group-id 5`**==, ==**`set password Fortinet`**==, ==**`set hbdev port7 0`**==, ==**`set session-pickup enable`**==, ==**`set override disable`**==, ==**`set priority 100`**==, and ==**`end`**== is used for **manually configuring all the necessary parameters for the FortiGate to operate in an Active-Passive High Availability (HA) cluster**.
    
- The command sequence ==**`config system ha`**==, followed by ==**`set ha-mgmt-status enable`**== and ==**`set ha-mgmt-interface <port_name> <gateway_ip>`**==, is used for **enabling and reserving a specific interface for High Availability (HA) management access**.
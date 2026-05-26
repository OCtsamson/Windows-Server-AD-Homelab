# Setup Static IP and DNS on Windows Server

## Thought Process: 

- **Why did I set a static IP for this Windows Server?**
  - Research showed that it is best practice to use a static IP rather than DHCP for servers

Other devices and services need to reliably find the server at the same network address all the time

**DHCP can cause IP changes that break services, DNS records, authentication and connections. Clients use DNS to locate DC's**

- **How did I set the static IP for my server?**
  - I decided to use ipconfig in command prompt to look for the IP address that was made for me when I created the virtual machine. I did this for consistency 

- **What did I set DNS address to?**
  - I left it as preferred DNS because I wanted it to be configured as the loopback address (same as IP)
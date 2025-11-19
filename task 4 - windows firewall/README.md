# Setup and Use a Firewall (Windows)

**Objective**: Configure and test basic firewall rules to allow or block traffic  
**System**: Windows 11  
**Tool**: Windows Defender Firewall with Advanced Security

### Task Steps Completed (exactly as assigned)

- Opened firewall configuration tool → Run → wf.msc  
- Listed current firewall rules → Inbound and Outbound Rules  
- Added a rule to block inbound traffic on port 23  
- Tested the rule → `Test-NetConnection 127.0.0.1 -Port 23` → failed (blocked)  
- Removed the test block rule → original state restored  
- All GUI steps and screenshots attached  
- Summary of how firewall filters traffic → see below

### Summary: How a Firewall Filters Traffic
- A firewall examines every incoming and outgoing packet and matches it against a list of ordered rules. Each rule checks protocol (TCP/UDP), source/destination IP, and port numbers.  
- If a packet matches a rule → the specified action (allow or block) is applied.  
- If no rule matches → the default policy is applied (on Windows: block all unsolicited inbound traffic).  
- Rules are processed top-to-bottom. the first match wins.

Screenshots and detailed steps are in this repository.
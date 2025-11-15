# Local Network Open Ports Scan  

## Objective
Learn to discover open ports on devices in your local network to understand network exposure.

## Tools Used
- **Nmap**  
- **Wireshark** 

---

## Step-by-Step Execution

1. **Installed Nmap**   
2. **Local IP range** – `192.168.1.0/24` (found via `ipconfig`)  
3. **Scan command** – `nmap -sS 192.168.1.0/24`  
4. **Results** – see `scan_results.txt`  
5. **Packet capture** – started Wireshark on interface `Wi-Fi`, saved as `wireshark_capture.png`  
6. **Services research** – documented in `services_research.md`  
7. **Security risks** – documented in `security_risks.md`

---

## Summary of Open Ports

| IP Address      | Open Ports (TCP)         |
|-----------------|--------------------------|
| 192.168.x.x     | 53, 80, 443, 1900        |
| 192.168.x.x     | 135, 139, 445            |

---

## Files Included
- `scan_results.txt` – raw console output  
- `services_research.md` – common services  
- `security_risks.md` – risk analysis  
- `wireshark_capture.png` – wireshark live capture
- `commands.md` – commands used

---

**All steps completed.**
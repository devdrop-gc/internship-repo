# Potential Security Risks

| Port     | Risk                                      | Recommendation                                      |
|----------|-------------------------------------------|-----------------------------------------------------|
| 22       | Brute-force, weak keys                    | Use key auth, fail2ban, restrict IPs                |
| 80/443   | Exposed admin panels                      | Change default credentials, restrict to LAN         |
| 53       | DNS spoofing                              | Block external queries, use DNSSEC                  |
| 135      | MSRPC enumeration & exploits              | Disable if not needed; block externally             |
| 139      | NetBIOS name disclosure, SMB attacks      | Disable NetBIOS over TCP/IP                         |
| 445      | SMBv1 exploits (EternalBlue, etc.)        | Patch Windows, disable SMBv1, firewall rule         |
| 1900     | UPnP port forwarding                      | Disable UPnP on router                              |
| 5900     | VNC weak/no password                      | Disable or use strong password + SSH tunnel         |
| 9100     | Printer DDoS reflection                   | Firewall rule: allow only LAN                       |
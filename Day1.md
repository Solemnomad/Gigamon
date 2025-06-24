---
## Net Recon Methodology
* HostDiscovery
    * Ruby ping sweep (if ping available)
    * Nmap scan if no ping
* Port Discovery
    * nmap
    * nc scan script
* Port Validation
    * Banner grab using nc
* Follow-on actions based on ports found
    * if 21 or 80 __*wget -r IP_ADDRESS*__ (or) __*wget -r ftp://IP_ADDRESS*__ (or) Firefox
    * if 21 __*FTP [IP ADDR]*__ connects to ftp server:
          * __*passive*__
          * __*ls*__
          * __*get [filename*__
          * if 22 or 23 CONNECT and PASSIVE RECON

---


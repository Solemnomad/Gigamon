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

student1@gigamon.com





---
support@gigamon.com

Gigamon has virtual and cloud options


# Traffic options
* can filter basics or dedup
* operational technologies (AC system, video cameras, etc)

Gigamon can cover 4mb copper(ethernet) to 400gb fiber 

* can filter via vlan tags to determine where exactly traffic is coming from before aggregating it.
* deep packet inspection allowed WITH A LICENSE
* gigamon can generate metadata similar to suricata and zeek logs
* net flow is the summary of the traffic on the network. It loses some fidelity but takes less storage ( 
* can generate application level metadata
* Allows inline operations through the gigamon depending on where it is placed, that allows you to block traffic if wanted.
* TLS 1.3 diffy-hellman encryption can only be decrypted inline with inline bypass.
* GIGASTREAM = load balancing
* gigamon can use vsphere to deploy X for east/west traffic and fabric manager
* fail-to-wire (fail passthrough) is only on the module relays inside the gigamon. The ports inside the chassis itself does not have it.
* HC-1 supports up to 40G throughput of data
* HCT small version supports up to 20G throughput of data
* FabMan can save multiple configs and you can swap through them as needed.
^- SAME PLACE you can download configs in binary or text format

# Gigamon links
Gigamon community portal
* community.gigamon.com
### Documentation library, can download entire guide based on software version
* AFTER version 6.11, fabric manager has AI built in.
^ Can walk you through step by step for instructions.
### additional resources
validated designs to complete tasks related to/dealing with gigamon. Step by step instructions.
#### Fabric manager can be any version =+ the node. 

## More -> Software and release notes
^- CANNOT ACCESS IMBED. Call him for software we need and can get it dropped to DODsafe.

## Fabric Manager
* does not need a license if managing ONLY ONE node.
  
### flow maps
can configure with CLI, GUI, or the API through fabric manager

### licenses
fabric manager can store the configuration for nodes and those configurations as well as their own configs can be pushed to an outside location via scp or sftp (location saved)

# inventory tab
where your nodes are managed

** PAY ATTENTION TO YOUR PRIORITY OF FLOWMAPS INSIDE GIGAMON **

* With Inline Network pair ports instead of Network ports with Port Pair, you are able to apply a IPS or such on the IN ports. 
^- traffic then goes all the way through to the IPA in your network instead of only going through the Port Pair network ports and simply copying the traffic.

* when going through port pairs, you need to enable link failure propogation so that one side of customer devices sees when the other is down. 
^- turn this off to troubleshoot when one side is down.

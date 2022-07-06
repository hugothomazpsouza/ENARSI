# DMVPN Phase 3 with IPSec and IKEv1

Below is information about the goals, settings, EVE-NG file and diagram used.

## Goals:

- Step 1 - Setup Interfaces IP addresses and eBGP Session between HUB and Spokes to ISP. LAN is assiged to Loopback 0
- Step 2 - Enable the EIGRP process on Loopback and Tunnel interfaces.
- Step 3 - Create a Tunnel interface that belong to NBMA network space 
	 - 3.1 - HUB feature:
		- Define IP address, Tunnel source, mode GRE Multipoint and key
		- Enable NHRP (multicast, authentication, network-id and redirect)
		- EIGRP (Create a summary-addres to LANs network space and Disable splithorizon and next-hop-self)
		- MTU 1400
		- MSS 1360
	- 3.2 - Spokes feature:
		- Define IP address, Tunnel source, mode GRE Multipoint and key
		- Enable NHRP (nhs, nhs map, multicast, authentication, network-id and shortcut)
		- MTU 1400
		- MSS 1360

- Step 4 - Setup crypto isakmp, tranform-set and IPSec Profile
- Step 5 - Assign the IPSec profile to tunnel

## Settings

- Settings of each Routers localized in the directory "Settings_Routers"

## EVE-NG File

- Zip file to import to EVE-NG localized in the directory "EVE-File". Import the ZIP file on the EVE-NG.

## Diagram

- The diagram can be found in the "Diagram" directory.






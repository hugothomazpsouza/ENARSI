# MPLS L3VPN

Below is information about the goals, settings, EVE-NG file and diagram used.

## Goals:

- Step 1 - Setup MPLS + LDP + OSPF on the Service Provider CORE. P Routers are BGP-Free Core.
- Step 2 - Create a VRF + RD for each customer. Setup VRF on the ports of the PEs where it has connection with the CEs.
- Step 3 - Setup the eBGP session between PEs and CEs. Advertise the CEs LAN routes into BGP.
- Step 4 - Setup the iBGP session between PEs and enable the Address Family VPN.
- Step 5 - Setup the Router Targets (import/export/both).

## Settings

- Settings of each Routers localized in the directory "Settings_Routers"

## EVE-NG File

- Zip file to import to EVE-NG localized in the directory "EVE-File". Import the ZIP file on the EVE-NG.

## Diagram

- The diagram can be found in the "Diagram" directory.






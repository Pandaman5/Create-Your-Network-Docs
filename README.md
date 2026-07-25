# Create-Your-Network-Docs

## Address Table:
|   Host-Name   |  Area  |    IP-Address    |   Gateway   |   DHCP Range    |
|---------------|--------|------------------|-------------|-----------------|
|   Router-1    | Room 4 |  192.168.1.1/24  |      ?      | 192.168.1.0-255 |
|
| Workstation-4 | Room 4 |      *DHCP*      | 192.168.1.1 | 192.168.1.0-255 |
| Workstation-3 | Room 3 |      *DHCP*      | 192.168.1.1 | 192.168.1.0-255 |
| Workstation-2 | Room 2 |      *DHCP*      | 192.168.1.1 | 192.168.1.0-255 |
|   Router-2    | Room 1 |  192.168.0.1/24  | 192.168.1.1 | 192.168.1.0-255 |
| Workstation-1 | Room 1 | 192.168.0.50/24  | 192.168.0.1 | 192.168.0.0-255 |
|   Server-1    | Room 1 | 192.168.0.100/24 | 192.168.0.1 | 192.168.0.0-255 |
|   Ubuntu-VM   | Room 1 | 192.168.0.110/24 | 192.168.0.1 | 192.168.0.0-255 |

## Network Devices:
|   Host-Name   |     Type     | Management IP |         Model         | Location  |      Purpose       |
|---------------|--------------|---------------|-----------------------|-----------|--------------------|
|   Router-1    |    Router    |  192.168.1.1  |   EERO 6+ (R010001)   |  Room 4   |    Edge Router     |
|   Switch-1    |    Switch    |   Unmanaged   | Netgear GS108 Switch  |  Room 4   | Edge Router Switch |
|   Printer-1   |   Printer    | 192.168.1.100 | HP LaserJet Pro M402n |  Room 3   |   Laser Printer    |
|   Router-2    |    Router    |  192.168.0.1  |  TP-Link Archer AX23  |  Room 1   |  Router/Switch/AP  |
|   Server-1    |    Server    | 192.168.0.100 |  HP Z800 Workstation  |  Room 1   |   Virtualization   |
|     AP-1      | Access Point |  192.168.1.1  |   EERO 6+ (R010001)   | Main Room |    Acess Point     |

# Create-Your-Network-Docs

## Address Table:
|   Host-Name   |  Area  |    IP Address    |   Gateway   |   DHCP Range    |
|---------------|--------|------------------|-------------|-----------------|
|   Router-1    | Room 4 |  192.168.1.1/24  |      ?      | 192.168.1.0-255 |
|   Switch-1    | Room 4 |    Unmanaged     | 192.168.1.1 | 192.168.1.0-255 |
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

## Network Services:
Seeing as this is a home network, the network services configures are limited, with most services being configured by Valley Fibre. The edge Router-1 and Router-2 are configured as DHCP servers and with DNS services for connected devices. 

## Device Configuration:
Device configuration on each device are set up at the discretion of the user. As this is a small home network, VLAN's and routing configuration's are left mostly default. I have configured network devices I own. All logins and usernames/passwords for my devices are saved on my personal BitWarden account. Here are some examples of device configuration:
| Host-Name |      OS       |  IP Address   | Backups |
|-----------|---------------|---------------|---------|
| Router-2  |  Windows 10   |  192.168.0.1  | Monthly |
| Server-1  | Proxmox 9.2.1 | 192.168.0.100 | Monthly |
| Ubuntu-VM | Ubuntu 26.04  | 192.168.0.110 | Monthly |

## Revision History"
Server-1:
|     Date      | Change |
|---------------|--------|
| June 6. 2026  | Installed Proxmox 9.1.1                 |
| June 16, 2026 | Configured Ubuntu-VM                    |
| June 27, 2026 | Deleted OS, and installed Proxmox 9.2.1 |
| July 4, 2026  | Recreated Ubuntu-VM                     |

## Diagrams:
Both Physical and Logical topology diagrams are included in this repository in the "Diagrams" folder.

### Physical Topology:
![Physical network topology](https://github.com/Pandaman5/Create-Your-Network-Docs/blob/main/Diagrams/Lesson%205%20-%20Create%20Your%20Network%20Docs%20(Physical).PNG)

### Logical Topology:
![Logical network topology](https://github.com/Pandaman5/Create-Your-Network-Docs/blob/main/Diagrams/Lesson%205%20-%20Create%20Your%20Network%20Docs%20(Logical).PNG)


# Cisco IOS CLI cheat sheet

## Modes

| Mode           | Description |
| ---            | --- |
| `>`            | User EXEC mode |
| `#`            | Privileged EXEC mode |
| `(config)#`    | Global configuration mode |
| `(config-if)#` | Interface configuration mode |

## Passwords

| Mode      | Command                       | Description |
| ---       | ---                           | --- |
| (config)# | `enable password <password>`  | Set plain text password to <password> |
| (config)# | `service password-encryption` | Use Cisco's Type 7 encoding |
| (config)# | `enable secret <password>`    | Set MD5 hashed password to <password> and disable old passwords |

## Basics

| Mode        | Command                                              | Description |
| ---         | ---                                                  | --- |
| >           | `enable`                                             | Change to Privileged EXEC mode |
|             | `exit`                                               | Exit current mode |
|             | `no <command>`                                       | Disable a feature/function or reverse the action of <command> |
| #           | `configure terminal`                                 | Enter Privilleged EXEC mode |
| #           | `show running-config`                                | Show current config |
| #           | `show startup-config`                                | Show startup config |
| #           | `write`                                              | Save running-config as startup-config |
| #           | `write memory`                                       | Save running-config as startup-config |
| #           | `copy running-config startup-config`                 | Save running-config as startup-config |
| #           | `ping <ip_address>`                                  | Ping <ip_address> |
| (config)#   | `shutdown`                                           | Disable interface |
| #           | `show mac address-table`                             | Show the MAC address table |
| (config)#   | `clear mac address-table`                            | Manually clear the MAC address table |
| (config)#   | `clear mac address-table dynamic <interface>`        | Clear MAC address table entry for <interface> interface |
| (config)#   | `do <command>`                                       | Run <command> in Privileged EXEC mode |
| #           | `show arp`                                           | View the ARP table and show all ARP entries |
| #           | `show ip interface brief`                            | Show interfaces status and configured IP addresses |
| (config)#   | `interface <interface_name>`                         | Enter <interface_name> config mode |
| (config)#   | `interface range <interface_start> <interface_stop>` | Enter interface config mode for all interfaces (including) <interface_start> through <interface_stop> |
| (config)#   | `ip address <ip_address> <subnet_mask>`              | Configure interface IP address |

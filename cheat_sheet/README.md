# Cisco IOS CLI cheat sheet

## Modes

| Mode           | Description |
| --- | --- |
| `>`            | User EXEC mode |
| `#`            | Privileged EXEC mode |
| `(config)#`    | Global configuration mode |
| `(config-if)#` | Interface configuration mode |

## Basics

| Mode      | Command                              | Description |
| :-: | --- | --- |
| >         | `enable`                             | Change to Privileged EXEC mode |
| #         | `configure terminal`                 | Enter Privilleged EXEC mode |
| (config)# | `interface <interface_name>`         | Enter <interface_name> config mode |
|           | `exit`                               | Exit current mode |
| #         | `show running-config`                | Show current config |
| #         | `show startup-config`                | Show startup config |
| #         | `write`                              | Save running-config as startup-config |
| #         | `write memory`                       | Save running-config as startup-config |
| #         | `copy running-config startup-config` | Save running-config as startup-config |

## Passwords

| Mode      | Command                       | Description |
| --- | --- | --- |
| (config)# | `enable password <password>`  | Set plain text password |
| (config)# | `service password-encryption` | Use Cisco's Type 7 encoding |
| (config)# | `enable secret <password>`    | Set MD5 hashed password and disable old passwords |

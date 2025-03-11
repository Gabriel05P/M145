# M145

**Aufgaben Cisco Packet Tracer**

## Aufgabe 02:

How many Fast Ethernet interfaces does the switch have?

24 FastEhternet interfaces
How many Gigabit Ethernet interfaces 

does the switch have?
2 Gigabit Ethernet

What is the range of values shown for the vty lines?
line vty 0 4
line vty 5 15
range of 0-15


## Aufgabe 04:


| Feld              | Wert             |
|-------------------|------------------|
| Destination MAC  | 000C:85CC:1DA7   |
| Source MAC       | 00D0:D311:C788   |
| Source IP        | 172.16.31.5      |
| Destination IP   | 172.16.31.2      |



| At Device     | Dest. MAC       | Src MAC        | Src IPv4     | Dest IPv4    |
|--------------|----------------|---------------|-------------|-------------|
| 172.16.31.5  | 000C:85CC:1DA7  | 00D0:D311:C788 | 172.16.31.5 | 172.16.31.2 |
| Switch1      | 000C:85CC:1DA7  | 00D0:D311:C788 | 172.16.31.5 | 172.16.31.2 |
| Hub          | N/A             | N/A            | 172.16.31.5 | 172.16.31.2 |
| 172.16.31.2  | 00D0:D311:C788  | 000C:85CC:1DA7 | 172.16.31.2 | 172.16.31.5 |
| Router       | 000C:85CC:1DA7  | 00D0:D311:C788 | 172.16.31.5 | 172.16.31.2 |

**Step 2**

| At Device     | Dest. MAC       | Src MAC        | Src IPv4     | Dest IPv4    |
|--------------|----------------|---------------|-------------|-------------|
| 172.16.31.3  | 000C:85CC:1DA7  | 0060:7036:2849 | 172.16.31.2 | 172.16.31.3 |
| Switch1      | 000C:85CC:1DA7  | 0060:7036:2849 | 172.16.31.2 | 172.16.31.3 |
| Hub          | N/A             | N/A            | 172.16.31.2 | 172.16.31.3 |
| 172.16.31.2  | 0060:7036:2849  | 000C:85CC:1DA7 | 172.16.31.3 | 172.16.31.2 |

| At Device     | Dest. MAC       | Src MAC        | Src IPv4     | Dest IPv4    |
|--------------|----------------|---------------|-------------|-------------|
| 172.16.31.4  | 00D0:D311:C788  | 000C:CF0B:BC80 | 172.16.31.4 | 172.16.31.5 |
| Switch1      | 000C:CF0B:BC80  | 00D0:D311:C788 | 172.16.31.4 | 172.16.31.5 |
| Hub          | N/A             | N/A            | 172.16.31.4 | 172.16.31.5 |
| 172.16.31.5  | 000C:CF0B:BC80  | 00D0:D311:C788 | 172.16.31.4 | 172.16.31.5 |
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

### Part 2:

| At Device     | Dest. MAC        | Src MAC          | Src IPv4   | Dest IPv4  |
|-------------------|---------------------|----------------------|---------------|---------------|
| 172.16.31.5  | 00D0:BA8E:741A       | 00D0:D311:C788       | 172.16.31.5   | 10.10.10.2    |
| Switch1      | 00D0:BA8E:741A       | 00D0:D311:C788       | N/A           | N/A           |
| Router       | 0060:2F84:4AB6       | 00D0:588C:2401       | 172.16.31.5   | 10.10.10.2    |
| Switch0      | 0060:2F84:4AB6       | 00D0:588C:2401       | N/A           | N/A           |
| Access Point | N/A                  | N/A                  | N/A           | N/A           |
| 10.10.10.2   | 00D0:588C:2401       | 0060:2F84:4AB6       | 10.10.10.2    | 172.16.31.5   |

## Questions:

**Waren verschiedene Kabel-/Medientypen zur Verbindung der Geräte im Einsatz?**
Ja, es wurden sowohl kabelgebundene (Ethernet) als auch drahtlose Verbindungen verwendet.

**Haben die Kabel die Verarbeitung des PDU in irgendeiner Weise verändert?**
Nein, die Kabel beeinflussen die PDU nicht direkt, sondern lediglich die physische Übertragung der Daten.

**Hat der Hub Informationen verloren, die er empfangen hat?**
Nein, der Hub hat keine Informationen verloren. Er sendet jedoch alle eingehenden Pakete an alle angeschlossenen Geräte weiter, was zu Kollisionen und potenziellem Datenverlust führen kann.

**Was macht der Hub mit MAC- und IP-Adressen?**
Der Hub verarbeitet keine MAC- oder IP-Adressen intelligent. Er sendet einfach alle eingehenden Pakete an alle verbundenen Geräte weiter.

**Hat der drahtlose Access Point etwas mit den übermittelten Informationen gemacht?**
Ja, der Access Point hat das Signal von kabelgebundenen Geräten in ein drahtloses Signal umgewandelt und umgekehrt.

**Wurde während der drahtlosen Übertragung eine MAC- oder IP-Adresse verloren?**
Nein, die MAC- und IP-Adressen bleiben bei der Übertragung erhalten.

**Welche höchste OSI-Schicht wurde vom Hub und Access Point verwendet?**

    Der Hub arbeitet auf Schicht 1 (Physikalische Schicht).
    Der Access Point arbeitet auf Schicht 2 (Sicherungsschicht), da er MAC-Adressen verarbeitet.

**Hat der Hub oder Access Point jemals ein PDU repliziert, das mit einem roten „X“ abgelehnt wurde?**
Nein, sie replizieren nur gültige PDUs.

**Welche MAC-Adresse erschien zuerst im PDU-Detail-Tab, die Quell- oder die Zieladresse?**
Die Quell-MAC-Adresse erscheint zuerst.

**Warum erscheinen die MAC-Adressen in dieser Reihenfolge?**
Weil das Paket von der Quelle zur Destination gesendet wird, und die MAC-Adresse der Quelle zuerst verarbeitet werden muss.

**Gab es ein Muster in der MAC-Adressierung der Simulation?**
Ja, Geräte desselben Herstellers hatten oft ähnliche MAC-Präfixe.

**Haben die Switches jemals ein PDU repliziert, das mit einem roten „X“ abgelehnt wurde?**
Nein, Switches leiten Pakete nur an bekannte MAC-Adressen weiter.

**Wo änderten sich die MAC-Adressen plötzlich, wenn das PDU zwischen den Netzwerken 10.x.x.x und 172.x.x.x gesendet wurde?**
Beim Router, da er MAC-Adressen für jedes verbundene Netzwerksegment neu setzt.

**Welches Gerät verwendet MAC-Adressen, die mit 00D0:BA beginnen?**
Vermutlich ein bestimmter Netzwerk-Switch oder ein anderer Netzwerkknoten.

**Zu welchen Geräten gehörten die anderen MAC-Adressen?**
Jede MAC-Adresse gehört entweder zu einem Endgerät (PC, Server) oder zu einem Netzwerkgerät (Router, Switch, Access Point).

**Haben sich die Quell- und Ziel-IP-Adressen in irgendeinem der PDUs geändert?**
Nein, die Quell- und Ziel-IP-Adressen bleiben in einem IP-Paket konstant.

**Wenn du die Antwort auf ein Ping verfolgst (Pong), tauschen dann die Quell- und Ziel-IP-Adressen die Plätze?**
Ja, beim Antwortpaket (Pong) werden die IP-Adressen vertauscht – die ursprüngliche Ziel-IP wird zur Quell-IP und umgekehrt.

**Gab es ein Muster in der IPv4-Adressierung der Simulation?**
Ja, das 172.x.x.x-Netzwerk und das 10.x.x.x-Netzwerk wurden durch den Router getrennt.

**Warum müssen unterschiedliche IP-Netzwerke verschiedenen Router-Ports zugewiesen werden?**
Weil Router Netzwerke verbinden und IP-Weiterleitung nur zwischen unterschiedlichen Netzwerken funktioniert.

**Was wäre anders, wenn die Simulation mit IPv6 statt IPv4 konfiguriert wäre?**

    IPv6-Adressen wären länger und hexadezimal dargestellt.
    Es gäbe keine ARP-Abfragen, da IPv6 Neighbor Discovery Protocol (NDP) verwendet.
    Automatische Adresskonfiguration wäre möglich, da IPv6 Stateless Address Autoconfiguration (SLAAC) unterstützt.
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

## Aufgabe 5:

## Part 1: Examine an ARP Request

### Step 1: Generate ARP Requests**

**a. Ist die Ziel-MAC-Adresse in der Tabelle oben aufgeführt?**

Ja, die MAC-Adresse des Ziels (172.16.31.3) 0060.7036.2849 ist in der Tabelle aufgeführt.

**b. Wie viele Kopien des PDU hat Switch1 erstellt?**

Es wurden 3 Kopien von Switch1 erstellt.

**c. Welche IP-Adresse hat das PDU akzeptiert?**

Die IP-Adresse 172.16.31.3, da sie der Ziel-IP-Adresse entspricht.

**d. Was passierte mit den Quell- und Ziel-MAC-Adressen?**

Die Quell-MAC-Adresse war die MAC-Adresse von 172.16.31.2 (000C.85CC.1DA7).
Die Ziel-MAC-Adresse wurde als Broadcast (FFFF.FFFF.FFFF) gesetzt, da die ARP-Anfrage an alle Geräte im Netzwerk gesendet wird.

**e. Wie viele Kopien des PDU hat der Switch während der ARP-Antwort erstellt?**

Da die ARP-Antwort ein Unicast-Paket ist, wird es nur an den anfragenden Host gesendet. Der Switch hat also eine einzige Kopie des PDUs weitergeleitet.

## Part 2: Examine a Switch MAC Address Table

### Step 1: Generate additional traffic to populate the switch MAC address table.

**Wie viele Antworten wurden gesendet und empfangen?**

Beim Ping von 172.16.31.2 - 172.16.31.4 und 10.10.10.2 - 10.10.10.3 werden vier ICMP-Antworten gesendet und empfangen.

### Step 2: Examine the MAC address table on the switches.

**a. Stimmen die Einträge in der MAC-Adressentabelle mit der Tabelle oben überein?**

Ja, die MAC-Adressen stimmen mit den Einträgen der Netzwerkgeräte überein.


**b. Warum sind zwei MAC-Adressen mit einem Port verbunden?**

Das geschieht normalerweise, wenn ein Switch an ein anderes Netzwerkgerät angeschlossen ist, das mehrere MAC-Adressen verwendet (z. B. ein weiterer Switch, ein Router oder ein Access Point).
In diesem Fall würde der Switch lernen, dass mehrere MAC-Adressen über denselben Port erreichbar sind.

## Part 3: Examine the ARP Process in Remote Communications

### Step 1: Generate traffic to produce ARP traffic.

**a. Was ist die IP-Adresse des neuen ARP-Tabelleneintrags?**

Nachdem ping 10.10.10.1 ausgeführt wurde und arp -a überprüft wird, ist ein neuer Eintrag mit der MAC-Adresse von 10.10.10.1 erschienen.

**b. Wie viele PDUs erscheinen nach arp -d und erneutem Ping?**

Zwei PDUs erscheinen

**c. Was ist die Ziel-IP-Adresse des ARP-Requests?**

Die Ziel-IP-Adresse des ARP-Requests ist die IP-Adresse des Standard-Gateways (Router) und nicht direkt 10.10.10.1.

**d. Warum ist die Ziel-IP-Adresse nicht 10.10.10.1?**

Das liegt daran, dass 172.16.31.2 und 10.10.10.1 sich in unterschiedlichen Netzwerken befinden.
Ein Host fragt per ARP nur nach MAC-Adressen im eigenen Subnetz.
Da 10.10.10.1 ausserhalb des Subnetzes 172.16.31.0 liegt, sendet der PC stattdessen einen ARP-Request an das Standard-Gateway (Router1), weil dieser für das Routing zuständig ist.

### Step 2: Examine the ARP table on Router1.

**a. Wie viele MAC-Adressen sind in der Tabelle? Warum?**

show mac-address-table auf Router1 zeigt wie viele adressen auf der Tabelle sind. Bei mir waren keine aufgelistet.der Router speichert nur MAC-Adressen für direkt verbundene Geräte.

**b. Gibt es einen Eintrag für 172.16.31.2 in der ARP-Tabelle (show arp)?**

Ja, da der Router eine ARP-Anfrage von 172.16.31.2 erhalten hat, speichert er dessen MAC-Adresse in der ARP-Tabelle.

**c. Was passiert beim ersten Ping, wenn der Router eine ARP-Anfrage beantworten muss?**

Der erste Ping schlägt oft fehl oder hat eine Verzögerung, weil der Router zuerst eine ARP-Anfrage senden muss, um die MAC-Adresse von 172.16.31.2 oder 10.10.10.1 zu lernen.
Sobald der Router die ARP-Antwort erhält, kann er den Ping weiterleiten.
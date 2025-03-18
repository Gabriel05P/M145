## Netzerkdokumentation richtig interpretieren


**Wie lautet die Netzwerkadresse vom Standort Samedan?**

- 192.168.3.0/24

**Auf welcher IP-Adresse befindet sich der AccessPoint in Bellinzona?**

- 192.168.4.30/24

**In welchem VLAN befinden sich die Arbeitsplatz-PCs?**

- Im VLAN-2, Office Port 1-23

**Über welche IP-Adresse erreicht man den Manageable-Switch am Standort Chur?**

- 192.168.2.253

**Welche IP-Adressen LAN-seitig und tunnelseitig ist der VPN-Gateway am Standort Bellinzona konfiguriert?**

- IP-Adresse tunnelseitig: 172.200.4.2
- IP-Adresse LAN-seitig: 192.168.4.1


**Wie lautet der am Standort Samedan an den Arbeitsplatz-PCs eingetragene Standardgateway?**

- 192.168.3.1

**Ein Aussendienstmitarbeiter benötigt Zugriff auf das Firmennetzwerk. Wie muss er seine VPN-SW IP-mässig konfigurieren?**

Er muss sich mit VPN-C Remote-Access verbinden und die IP sollte dynamisch zugewiesen werden, sobald die VPN-Verbindung hergestellt ist.

**Wer hat im Büro CAD Wasserbau die VoIP-Telefone installiert?**

- abisang hat die VoIP-Telefone installiert am 19.5.14
- E10/1, E10/3, E11/1, E13/3

**Wann wurde im Bistro der AccesPoint installiert?**

- Am 23.7.14 von rsauter E8/1

**Der IT-Mitarbeiter Rene Sauter (rsauter) verlässt die Firma. Welche Arbeiten bzw. Verantwortlichkeiten sind davon betroffen? Wen würden sie als zukünftigen Ansprechpartner bei Problemen vorschlagen?**

- Empfang EG Arbeitsplatz-PC 29.11.13, E1/11
- CAD Tiefbau CAD Workstation 13.08.13, E2/1
- Bauleitbüro MF-Kopierer 11.10.13, E3/2
- Bistro Access-Point 23.7.14, E8/1

Es gibt mehrere mögliche Kandidaten für die Aufgabe. Abisang hat vor allem VoIP-Telefone eingerichtet, was darauf hindeutet, dass er Erfahrung mit den Patchpanel-Anschlüssen besitzt. Rkundert hat sich hauptsächlich um Arbeitsplätze gekümmert, verfügt aber insgesamt über weniger Erfahrung. Blaeuchli hingegen hat sowohl Arbeitsplätze als auch einen Plotter eingerichtet, was auf eine breitere Kenntnis der Netzwerkinfrastruktur schließen lässt. Daher wäre entweder Blaeuchli aufgrund seiner vielseitigen Erfahrung oder Abisang wegen seiner Spezialisierung auf VoIP eine sinnvolle Wahl.


**Wieviele RJ45-Steckdosen stehen ihnen im Bauleiterbüro zur Verfügung und wieviele davon sind zurzeit noch nicht belegt?**

- Im Bauleiterbüro gibt es 8 RJ45-Steckdosen.
- Noch nicht belegt sind E3/1 und E6/2.

**Im Büro CAD Tiefbau muss ein weiteres VoIP-Telefon zur Verfügung stehen. Wie soll diese Verbindung gepatched werden? Verlangt wird die Patchpanelbelegung und der Switch-Port.**


- Laut der Belegungsliste sind im CAD Tiefbau bereits ein VoIP-Telefon auf Anschluss E2/3 sowie eine CAD-Workstation auf Anschluss E2/1 vorhanden. Anschluss E2/2 ist in der Liste nicht als belegt gekennzeichnet und kann daher für das neue Telefon genutzt werden.

- Das Kabel wird vom Patchpanel Port E2/2 zum entsprechenden Switch-Port für das VoIP-VLAN gepatcht. Da die    anderen VoIP-Telefone im Bauleiterbüro und CAD Tiefbau bereits auf VLAN-konfigurierten Ports laufen, sollte derselbe VLAN-Tag verwendet werden.

**Im Bistro soll eine Projektpräsentation stattfinden. Dafür muss ein Ethernetkabelverbindung bereitgestellt werden.**

Im Bistro stehen die Anschlüsse E9/1 und E9/2 zur Verfügung, da E8/1 bereits für einen Access Point belegt ist. Für die Projektpräsentation kann einer der freien Anschlüsse, beispielsweise E9/1 oder E9/2, genutzt werden. Die Verbindung muss am Patchpanel hergestellt und mit einem Switch-Port verbunden werden, der dem passenden VLAN zugewiesen ist. Vermutlich dem Office-Netzwerk.


**Im Büro CAD Wasserbau soll temporär ein weiterer Arbeitsplatz eingereichtet werden. Wie werden sie diese Aufgabe lösen?**

Die Anschlüsse E10/2, E10/4, E11/2 und E11/4 sind bereits für Arbeitsplatz-PCs reserviert. Da aktuell keine freien RJ45-Ports verfügbar sind, kann kein weiterer PC direkt angeschlossen werden. Eine mögliche Lösung wäre, einen kleinen unmanaged Switch (z. B. ein kompakter Netgear-Switch) an einen bestehenden Port anzuschließen, um zusätzliche Netzwerkanschlüsse bereitzustellen.

**Wie viele Switchs stehen ihnen am Standort Chur zur Verfügung?**

- in Chur 2 ZyXEL XGS1910-24 Switches

**Frau Sommer arbeitet an der CAD-Workstation und meldet ihnen, dass sie keine Verbindung ins Internet mehr hat. Was werden sie überprüfen?**

- Patchpanel & Verkabelung: Sicherstellen, dass E2/1 korrekt angeschlossen ist.
- Switch & VLAN: Prüfen, ob der richtige Switch-Port und VLAN konfiguriert sind.
- IP-Adresse: Überprüfung der IP-Vergabe (DHCP oder statisch).
- Gateway & DNS: Ping-Test zum Gateway und DNS-Server.
- Switch/Netzwerksegment: Falls mehrere Geräte betroffen sind, mögliche Switch- oder Routing-Probleme   untersuchen.

**Wie lautet die SSID des Churer-AccessPoint?**

- Die SSID steht nicht im Diagramm
- SSID steht für „Service Set Identifier“ und ist der Name eines Wi-Fi-Netzwerks. Wenn Sie die Liste der Wi-Fi-Netzwerke auf Ihrem Laptop oder Telefon öffnen, sehen Sie eine Liste von SSIDs. (In diesem Fall kann ich es anhand der Netzwerkdokumentation nicht auslesen)
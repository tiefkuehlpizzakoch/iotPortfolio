Step A:
Ich fand es sehr cool zu sehen, was andere Studierende in diesem Kurs schon gemacht haben und wie damit direkt tatsächliche praktische Probleme in Angriff genommen werden konnten. Vom „Harvestmate Smart Planter“ bis zum „Gesture Based Music Making“ ist mir sehr positiv aufgefallen, wie breit die umgesetzten Projekte variieren. 

Ich hätte sehr viel Lust, ein ähnliches Projekt umzusetzen, vielleicht auch etwas in die Richtung des „Harvestmate Smart Planter“. Ich fand die Idee von Vertical Farming schon immer sehr cool. Daran, und am Smart Planter inspiriert könnte ich mit gut vorstellen, eine Art “Blumentopf” zu entwickeln, welcher anhand von Feuchtigkeitssensoren im Boden und informationen über den Wasserbedarf der jeweiligen Pflanze, automatisch das gießen der Pflanze übernimmt. 

Step B:
Netzwerktechniker bevorzugen das 4-Schichten-TCP/IP-Modell, da es praxisnah ist und die tatsächliche Architektur des Internets beschreibt. In der Realität sind Layer 5,6,7: Session, Presentation, nach belieben von den Anwendungen implementiert. 

Step C:
Hands On:
1. IP: 192.168.178.173
IP home router: IP192.168.178.1
Netmask: 0xff000000

2. Anzahl Hops: 7
Private to Public: zwischen Hop 1 und 2

<img width="201" height="219" alt="image" src="https://github.com/user-attachments/assets/3d99a9e8-66d2-42db-8e58-a0057288649b" />


Guiding Questions:
Mich hat im Video vor allem die Richtung des "Harvestmate Smart Planter" gebracht, da ich Vertical Farming schon immer ziemlich cool fand. Ich hätte lust, so einen smarten Blumentopf als Projekt umzusetzen, der Pflanzen von alleine gießt. Dafür müssten Feuchtigkeitssensoren in der Erde ihre Daten an eine kleine Steuerung schicken, die den Wasserbedarf der Pflanze checkt und mit presets zum Wasserbadarf dieser Pflanze vergleicht. Jeder, der schwierigkeiten damit hat, seine Pflanzen regelmäßig zu gießen wäre hier ein potenziellen Nutzer.

2. Eine IP-Adresse kann man sich als Postanschrift eines Geräts im Netzwerk vorstellen. Die Subnetzmaske sagt dem Gerät, welcher Teil dieser Adresse für das gesamte Netzwerk steht und welcher für das spezifische Gerät. Zwei Geräte im selben lokalen Netz können nicht dieselbe IP haben, weil das zu einem Konflikt führt. Der Router wüsste dann nicht mehr, wem von beiden er die ankommenden Datenpakete zustellen soll.

3. Das OSI-Modell ist in der Theorie zwar nett, aber für kleine IoT-Geräte oft völlig übertrieben. Wenn ein Sensor nur zwei Bytes an Nutzdaten sendet, wie etwa eine Temperatur, oder einen Feuchtigkeitswert, würden die strengen Vorgaben der vielen Schichten riesigen Overhead durch unzählige Header erzeugen. Das frisst bei kleinen, batteriebetriebenen Sensoren viel zu viel Strom und Bandbreite, weshalb man in der Praxis Protokolle nutzt, die Schichten einfach zusammenfassen oder weglassen.

4. Wenn man HTTP nutzt, müsste jeder der 10 Sensoren eine direkte Verbindung zu jedem der 3 Displays aufbauen, was zu sehr viel Aufwand beim hinzufügen eines Gerätes oder beim Warten führt. Ein MQTT-Broker ist stattdessen ein zentraler Verteiler in der Mitte. Die Sensoren schicken ihre Daten einfach nur dorthinDas entkoppelt das System komplett und macht die Verwaltung deutlich effizienter.

5. Man kann aus dem eigenen Home-Office nicht direkt ein Gerät im WLAN eines Kommilitonen anpingen. Das liegt daran, dass unsere Heimnetzwerke private IPs nutzen, die im Internet nicht geroutet werden. Ein Mesh-Overlay wie Nebula ändert das, indem es ein verschlüsseltes, virtuelles Netz über das normale Internet legt. Es gibt den Geräten spezielle Overlay-IPs und lässt sie so direkt miteinander kommunizieren. 


Andere Notizen: 
Hosts
Host: send or receive traffic
Clients: initiates request
Server: responds to request
Specific to current communication
Server: Computer with software installed, to fullfill specific request.

IP Address: Needed to send & receive, identity of every host. Every request, and its answer stamped with src and dst ip address.
32 Bits. Every 8 places converted to corresponding decimal number. 
Hierarchy: Einzelne Teile der IP, zugeordnet zu bestimmten Gerätegruppen. 

Network: Transports traffic between Hosts. Logical grouping of hosts which require similar connectivity. 

Repeater: Because signal decays over great distance, Repeaters regenerate that Data.

Hub: Multi port repeater. 

Bridge: Only has two ports. Contains communication to necissary site. 

Switch: Combination of Hub and Bridge: Multiple devices connect, learn what host on what port. 

Router: Communication between different networks. Here security, fitering, redirecting should be added. Routing table: All networks a router knows. Has IP Address in every network it’s attached to. 
OSI Model:
Rules for Networking are known as the OSI Model. 
It’s a 7 Layer model:
Physical Layer (1): Bits are transported (Cables, Wifi)
Data Link (2): Interacts with Wire, Switches, 
Network Layer (3): IP Addresses, Routers, any device with IP address. 
Transport Layer (4): Distinguish data streams, Data has Layer 4 header. 
Layer 5,6,7: Session, Presentation, Application

<img width="468" height="541" alt="image" src="https://github.com/user-attachments/assets/1f4e450e-72d9-406a-86ee-3493a0b7eadf" />






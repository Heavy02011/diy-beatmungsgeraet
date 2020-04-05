<p align="center">
  <img src="images/logo.png">
</p>

# DIY-Beatmungsgerät

DIY Beatmungsgerät basierend auf einem Open Source und Open Hardware Entwurf. Der Grundstein wurde während des [#WirvsVirusHackathon](https://wirvsvirushackathon.org/) im März 2020 gelegt.

Das 3D-Modell des Beatmungsgerätes basiert auf Iteration #6 des Open Source Ventilator (OSV) Project, in gitlab unter https://gitlab.com/open-source-ventilator/OpenLung zu finden.


## Repository-Struktur

Wir arbeiten an verschiedensten Themen. Zum einen etwa an der Weiterentwicklung des Beatmungsgerätes, als auch an dessen Ansteuerung bzw. Regelung und weiterer Sensorik.

* [/ hardware / mass-airflow-model /](/hardware/mass-airflow-model/): Modelle für die Röhre eines Masseflusssensors
* [/ hardware / ventilator-model/](/hardware/ventilator-model/): das weiterentwickelte Modell des Beatmungsgerätes
* [/ software / mass-airflow-sensor / controller-software/](/software/mass-airflow-sensor/controller-software/): die Software, die auf der Plattform läuft, um den Luftmassesensor auszulesen (Mock-Up)
* [/ software / mass-airflow-sensor / sensor-software/](/software/mass-airflow-sensor/sensor-software/): die Software, die auf dem Sensor selbst läuft, der Luftmassesensor-Daten bereitstellt (Mock-Up)
* [/ software / ventilator-control/](/software/ventilator-control/): die Software für die Steuerungs-Plattform des Beatmungsgerätes


# Weiterführende Links
* [Homepage des WirvsVirus Hackathon](https://wirvsvirushackathon.org/)
* [Projekt-Vorstellung auf devpost.com](https://devpost.com/software/diy-beatmungsgerat)
* [Projekt-Vorstellung auf YouTube](https://www.youtube.com/watch?v=DzOd6LIBdXI)
* https://gitlab.com/open-source-ventilator/OpenLung
* [Discord-Server](https://discord.gg/GaRy2hR)
* [Phabricator (Taskboard)](https://diy-vent.vmcon.de/)

# Discord-Server
## Erste Schritte auf dem Discord
1. Vorstellung im Textkanal `Willkommen > #vorstellung`
2. Nickname ändern zu VornameNachname
	* rechter Mausklick auf deinen Namen in der rechten Spalte
	* im aufploppenden Menü auf `Nickname ändern`
3. Schau dich um. Wo kannst und willst du dich einbringen?
4. Für einen Überblick besuche die [GoogleDrive](https://drive.google.com/drive/folders/1Poj6eQrTGcuFaNvTQpUK7rhnsla_4bZM?usp=sharing ). Dort findest du die Tagesprotokolle der einzelnen Arbeitsgruppen zum Einlesen in deren bisherige Fortschritte.

## Tipps für besseres Arbeiten
Kommunikation und Diskussion funktionieren über Textkanäle schon ganz gut, aber oft noch besser per gesprochenem Wort. Dafür sind in jeder Kategorie **Sprachkanäle** eingerichtet, nutzt sie um gemeinsam an einer Sache zu arbeiten. Selbst wenn du zunächst allein in einem Sprachkanal sein solltest, deine Anwesenheit motiviert andere es dir gleich zu tun.

Kennst du schon den **Phabricator**? Er hilft bei der Übersicht der Aufgaben. Um ihn zu nutzen, registriere/melde dich bitte auf https://diy-vent.vmcon.de/ an. Ein detaillierte Anleitung dafür findest du [hier](https://docs.google.com/document/d/13HGdLew2o9hQ6I6csHRrQ5bDhwd4Uv7NS_OEr5iKHa8/edit#heading=h.q1sumqpr1ip0).

Das **offizielle Github-Repository** ist [hier](https://github.com/DIY-Beatmungsgerat/diy-beatmungsgeraet) zu finden. Nutzt und erweitert es und stellt pullrequests wenn ihr Fortschritte macht.

**Servergruppen** sind ein tolles Ding. Nicht nur für das Gruppengefühl, sondern auch um zu Zeigen in welcher Arbeitsgruppe man tätig ist. Das erleichtert die Kommunikation und es ist auf einen Blick ersichtlich wer bezüglich einer Arbeitsgruppe und Fagen dazu ansprechbar ist. Im Textkanal `#info-brett` findest du einen Beitrag, über den du dich einer oder mehrere Arbeitsgruppen zuweisen kannst. Bist du keiner Arbeitsgruppe zugeordnet, hast du in allen Kanälen nur Leserechte.

# Arbeitsgruppen
Die hier beschriebenen Arbeitsgruppen sind analog zu den Nutzergruppen des Discord-Servers.

## Kommunikation
Die Arbeitsgruppe Kommunikation beinhalte die Administration und Füllung der Website, die Verwaltung des Discord-Servers, die Öffentlichkeitsarbeit per Twitter und die Pflege der Presse- und Behördenkontakte. Da die Teilbereiche eng miteinander arbeiten und sich zum Teil auch überschneiden, wurde von einer kleinteiligeren Aufteilung abgesehen.

## Konstruktion 1 -- Motorisch betriebener Beatmungsbeutel
## Konstruktion 2 -- Motorisch betriebener Beatmungsbeutel - Alternative: Druckluftbetrieb
## Konstruktion 3 -- Kolbenpumpe
Ausgangspunkt für diese Konstruktion ist die Überlegung, dass Ambu-Beutel zwar ganz wichtige Vorteile (grundsätzliche Verfügbarkeit und Zertifizierung für Notbeatmung), aber auch zentrale Nachteile haben. Dazu gehört, dass sie in Zeiten dieser Krise bereits zu den knappen Gütern gehören und vielfach nicht mehr lagerhaltig zur Verfügung stehen, dass sie nur für eine äußerst begrenzte Standzeit (wenige Stunden Einsatz) gebaut sind und dass ihre automatische mechanische Betätigung möglicherweise doch nicht so einfach ist, wie zunächst angenommen.

Die Konstruktion einer Kolbenpumpe erscheint auf den ersten Blick etwas aufwändiger. Vorhandene und im medizinischen Prozess zertifizierte Bauteile sind den im Moment beteiligten Entwicklern nicht bekannt (und auch nicht umfangreich recherchiert worden). Vorteile einer Kolbenpumpe ist die jederzeitige relativ genaue Kenntnis über das „eingeblasene“ Volumen über den Verfahrweg des Kolbens im Zylinder.

Voraussetzung für eine sinnvolle Konstruktion ist der Antrieb des Kolbens über einen Spindelantrieb. Erste Überlegungen zu einem Kurbelantrieb wurden schnell verworfen, weil dabei das Hubvolumen mit einem zweiten Aktor verändert werden müsste.

## Onboarding
Die Arbeitsgruppe bewahrt den Überblick über unsere Mitglieder. Für alle Fragen rund um das „Personalmanagement“ sind sie die richtige Ansprechpartner. Zudem versuchen sie gezielt zu vermitteln, sodass sich jede und jeder entsprechend der eigenen Fähigkeiten optimal einbringen kann.

## Produktion
## Elektrik
## Sensorik
## Steuerung/Controller
## Userinterface
## Testing
## Management
## Requirements und Risiken
- [Requirements_and_tracking_v01_draftD](https://docs.google.com/spreadsheets/d/1g51Zr3aXuJa8Xe4WVbXgiYnll-a5mOB1ONs-IWp97Ys/edit#gid=2056750683)
- [PHA - Preliminary hazard analysis](https://docs.google.com/spreadsheets/d/1g51Zr3aXuJa8Xe4WVbXgiYnll-a5mOB1ONs-IWp97Ys/edit#gid=1530841219)
## Fundraising
## Springer

# Regelmäßige Berichte der Arbeitsgruppen
Bitte **jeden Abend um gegen 18:00** in die [GoogleDrive](https://drive.google.com/drive/folders/1Poj6eQrTGcuFaNvTQpUK7rhnsla_4bZM?usp=sharing ) einen kurzen Bericht zum aktuellen Stand machen.
Entweder Textdatei oder Präsentation. Ziel ist, dass das Managementteam und andere Teams sehen können wo ihr steht und auch das Neulinge sich schnell einlesen und zurechtfinden können.

# Regelmäßige Calls
- das Kernteam hat **Dienstags und Donnerstags 20:00** eine Videokonferenz (jeder darf zuhören). Protokoll im Protokoll Ordner.
- andere Teams legen eigenverantwortlich ihre regelmäßigen Runden fest und schreiben darüber auch Protokoll.

# FAQ und Wegweiser
hier faq von der webseite und dein "HOWTO Start"

# Tools

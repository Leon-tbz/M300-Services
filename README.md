# M300-Services
Modul 300
---
**1. Apache Webserver automatisiert aufsetzen**
Um den Automatisierungsgrad von Vagrant im Rahmen dieser Dokumentation etwas besser hervorzuheben, richten wir eine VM, dass sie direkt mit einem vorinstallierten Apache-Webserver startet. Dazu können wir im Vagrantfile den Code etwas leicht abändern und direkt auf Bash-Ebene mit einfachen Befehlen arbeiten.

Nachfolgend wird die VM mit einem bereits abgeänderten File bzw. VM aus dem M300-Repository erstellt:

Terminal (Bash) öffnen
In das M300-Verzeichnis (/M300/vagrant/web) wechseln:

 - $ cd Pfad/zum-M300-Verzeichnis/vagrant/web

VM erstellen und starten:

- $ vagrant up

Webbrowser in der VM öffnen und prüfen, ob der Standard-Content des Webservers unter "http://127.0.0.01:8080" (localhost) erreichbar ist
Im Ordner /web die Hauptseite index.html editieren bzw. durch eine andere ersetzen (z.B. HTML5up-Themplate) und das Resultat überprüfen
Abschliessend kann die VM wieder gelöscht werden:

- $ vagrant destroy -f

Vagrant ist nun komplett einsatzfähig!

---

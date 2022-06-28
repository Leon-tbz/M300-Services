---
# LB2-Mailserver mit Docker aufsetzen
---
In diesem Projekt werden wir einen Container erstellen auf dem schlussendlich ein voll funktionstüchtigen Owncloud Server mit SQL Datenbank anbindung läuft wird auf dem man Zentral über Web-Interface monitoren und Anpassen kann. Dabei werde ich in diesem GitHub Repo erklären und beschreiben wie wir den Server aufgesetzt haben und was die Funktionen dieses Dienstes sind.

---
# Was ist Owncloud?
---
![grafik](Owncloud.png))

OwnCloud ist eine freie Software für das Speichern von Daten (Filehosting) auf einem eigenen Server. Bei Einsatz eines entsprechenden Clients wird dieser automatisch mit einem lokalen Verzeichnis synchronisiert. Dadurch kann von mehreren Rechnern auf einen konsistenten Datenbestand zugegriffen werden. Das Projekt wurde im Januar 2010 vom KDE-Entwickler Frank Karlitschek ins Leben gerufen, um eine freie Alternative zu kommerziellen Anbietern eines Cloud-Service zu schaffen. Im Gegensatz zu kommerziellen Speicherdiensten kann ownCloud auf einem privaten Server oder Webspace installiert werden.

---

Folgende Features sind inbegriffen:

1. Zugriff auf Ihre Daten:
Speichern Sie alle Ihre Dokumente, Ordner, Kontakte, Fotoalben, Kalender und andere Informationen auf einem Server Ihrer Wahl.
Sie können einen Desktop, ein mobiles Gerät oder einen Webbrowser verwenden, um auf diesen Ordner zuzugreifen.
Sie können jederzeit und von jedem Ort aus auf Ihre Daten zugreifen.


2. Synchronisation der Daten
Synchronisieren Sie die Kalender, Kontakte, Fotoalben und andere Daten Ihrer Geräte.

3. Daten Verfügbar machen.
Greifen Sie auf Ihre neuesten Fotogalerien, Kalender, Musik und andere Inhalte zu, indem Sie Ihre Daten für andere freigeben.
Teilen Sie sie entweder offen oder heimlich.
Ihre Daten gehören Ihnen und Sie können sie verwenden, wie Sie wollen. 

4. Versionierung bei Änderungen einer Datei

5. Verschlüsselung der Daten
Wenn die Verschlüsselungsanwendung aktiviert ist, werden alle auf dem ownCloud-Server gespeicherten Dateien mit Ihrem Passwort verschlüsselt.

6. Hochladen per Drag & Drop

7. Anwendungs-API's
Neue, öffentlich definierte APIs machen die Erstellung von Anwendungen für ownCloud viel einfacher und ermöglichen zusätzliche Funktionen und einen stabilen Integrationspunkt für zukünftige Versionen.

8. Migration und Backup Funktionen

9. Protokollierung
Owncloud kann sowohl in Syslog-Protokolldateien als auch in die bestehende ownCloud-Protokolldatei schreiben.

---
# Umsetzung
---

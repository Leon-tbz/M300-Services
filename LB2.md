---
# LB2-Mailserver mit Docker aufsetzen
---
In diesem Projekt werden wir einen Container erstellen auf dem schlussendlich ein voll funktionstüchtigen Owncloud Server mit SQL Datenbank anbindung läuft wird auf dem man Zentral über Web-Interface monitoren und Anpassen kann. Dabei werde ich in diesem GitHub Repo erklären und beschreiben wie wir den Server aufgesetzt haben und was die Funktionen dieses Dienstes sind.

---
# Was ist Owncloud?
---
![grafik](logo.png))

OwnCloud ist eine freie Software für das Speichern von Daten (Filehosting) auf einem eigenen Server. Bei Einsatz eines entsprechenden Clients wird dieser automatisch mit einem lokalen Verzeichnis synchronisiert. Dadurch kann von mehreren Rechnern auf einen konsistenten Datenbestand zugegriffen werden. Das Projekt wurde im Januar 2010 vom KDE-Entwickler Frank Karlitschek ins Leben gerufen, um eine freie Alternative zu kommerziellen Anbietern eines Cloud-Service zu schaffen. Im Gegensatz zu kommerziellen Speicherdiensten kann ownCloud auf einem privaten Server oder Webspace installiert werden.

---

Folgende Features sind inbegriffen:

- 1. Zugriff auf Ihre Daten:
Speichern Sie alle Ihre Dokumente, Ordner, Kontakte, Fotoalben, Kalender und andere Informationen auf einem Server Ihrer Wahl.
Sie können einen Desktop, ein mobiles Gerät oder einen Webbrowser verwenden, um auf diesen Ordner zuzugreifen.
Sie können jederzeit und von jedem Ort aus auf Ihre Daten zugreifen.


- 2. Synchronisieren Sie Ihre Daten
Synchronisieren Sie die Kalender, Kontakte, Fotoalben und andere Daten Ihrer Geräte.
Holen Sie sich jederzeit die aktuellste Version Ihrer Dateien mit dem Desktop-, Web- oder Mobil-Client Ihrer Wahl. Dies gilt auch für Ordner mit einem, zwei und mehr Ordnern.


- 3. Machen Sie Daten verfügbar.
Greifen Sie auf Ihre neuesten Fotogalerien, Kalender, Musik und andere Inhalte zu, indem Sie Ihre Daten für andere freigeben.
Teilen Sie sie entweder offen oder heimlich.
Ihre Daten gehören Ihnen und Sie können sie verwenden, wie Sie wollen. 


- 4. Versionierung
Hat jemand eine Änderung an einer freigegebenen Datei vorgenommen, die Ihnen nicht gefällt, oder haben Sie versehentlich einen Teil der Datei gelöscht, den Sie benötigen? Wenn die Versions-Anwendung aktiviert ist, speichert ownCloud automatisch alte Dateiversionen - Sie legen fest, wie viel gespeichert werden soll. Wenn Sie zurückkehren möchten, fahren Sie einfach mit dem Mauszeiger über Ihre Datei und gehen Sie zu einer früheren Version zurück.

- 5. Verschlüsselung
Möchten Sie sicherstellen, dass Ihre Dateien auf dem Server sicher bleiben? Wenn die Verschlüsselungsanwendung aktiviert ist, werden alle auf dem ownCloud-Server gespeicherten Dateien mit Ihrem Passwort verschlüsselt. Dies ist hilfreich, wenn Sie Ihre Dateien auf einem nicht vertrauenswürdigen Speicher außerhalb des ownCloud-Servers speichern. Wenn Sie zusätzlich eine SSL-Verbindung herstellen, sind Ihre Dateien sowohl in Bewegung als auch im Ruhezustand sicher.

- 6. Hochladen per Drag & Drop
Sie arbeiten an einem Computer und möchten nicht den gesamten ownCloud-Client installieren? Melden Sie sich einfach in einem Webbrowser bei ownCloud an und ziehen Sie Ihre Dateien per Drag and Drop von Ihrem Desktop in das gewünschte Zielverzeichnis im Webbrowser. Sie werden dann automatisch auf den Server hochgeladen.

- 7. Thematisierung
Möchten Sie, dass ownCloud wie der Rest Ihrer Website aussieht und sich anfühlt? Nutzen Sie die neue Funktion des Theming-Verzeichnisses. Jeder Stil oder jedes Bild, das Sie in diesem Verzeichnis ablegen, wird anstelle der ownCloud-Standardschriftarten, -farben und -symbole verwendet.

- 8. Viewer für ODF-Dateien
Möchten Sie Dateien im Open Document Format lesen, ohne sie herunterzuladen? Aktivieren Sie diese Anwendung und Sie können auf jedes ODF-formatierte Dokument (.odt, .odp, .ods) klicken und es in Ihrem Webbrowser lesen, ohne es herunterladen zu müssen.

- 9. Anwendungs-API's
Möchten Sie ownCloud um Funktionen erweitern? Neue, öffentlich definierte APIs machen die Erstellung von Anwendungen für ownCloud viel einfacher und ermöglichen zusätzliche Funktionen und einen stabilen Integrationspunkt für zukünftige Versionen.

- 10. Migration und Backup
Haben Sie mehrere ownCloud-Instanzen, vielleicht eine primäre und eine Backup-Installation? Jetzt können Sie Ihre ownCloud-Benutzerkonten ganz einfach zwischen den ownCloud-Instanzen verschieben und bei Bedarf ein Backup bereithalten.

- 11. Aufgaben
Möchten Sie die Übersicht über Ihre wichtige Aufgabenliste behalten? Mit der Tasks-Anwendung können Sie Ihre Aufgabenlisten ganz einfach mit Ihrer ownCloud-Instanz synchronisieren.

- 12. Anwendungsspeicher
Möchten Sie eine der vorhandenen Anwendungen zu ownCloud hinzufügen? Aktivieren Sie einfach eine neue Anwendung in den Einstellungen, und sie wird automatisch heruntergeladen und in Ihrer ownCloud-Instanz installiert.

- 13. Kalender
Möchten Sie Ihren Kalender mit anderen ownCloud-Nutzern teilen? Aktivieren Sie die Kalenderanwendung, öffnen Sie Ihren Kalender, wählen Sie Teilen und wählen Sie die gewünschten Benutzer oder Gruppen. Im Handumdrehen können Sie Ihren wichtigen Kalender und wichtige Ereignisse freigeben.

- 14. Datei-Benachrichtigungen
Jetzt können Sie andere benachrichtigen, wenn eine Datei geteilt wird. Das macht es schneller und einfacher, diese Dokumente, Heimvideos und was auch immer Sie sonst noch wollen, zu teilen.

- 15. Galerien
Möchten Sie eine bessere Kontrolle über Ihre freigegebene Fotogalerie? Jetzt können Sie die ownCloud-Fotoverzeichnisse und die Sortierreihenfolge festlegen, Ihre Galerien an beliebige E-Mail-Adressen weitergeben und bestimmen, ob diese die Fotos mit anderen teilen können.

- 16. Externer Speicher
Möchten Sie an einem Ort auf alle Ihre Gdrive- und Dropbox-Dateien zugreifen? Dann sollten Sie sich diese neue experimentelle Funktion ansehen. Wenn Sie die Anwendung für externen Speicher aktivieren, können Sie Ihren externen Speicher als Ordner innerhalb Ihrer ownCloud-Instanz einbinden und über eine einzige Schnittstelle auf alle Ihre Dateien zugreifen.

- 17. Protokollierung
Möchten Sie ownCloud in Ihren bestehenden Syslog-Dienst integrieren? Jetzt kann ownCloud sowohl in Syslog-Protokolldateien als auch in die bestehende ownCloud-Protokolldatei schreiben.

- 18. LDAP/Active Directory
Möchten Sie ownCloud-Benutzer über ein Verzeichnis verwalten? Mit ownCloud können Administratoren jetzt Benutzer und Gruppen von ihrer LDAP- oder AD-Instanz aus verwalten.
---
# Umsetzung
---

---
# LB2-Mailserver mit Docker aufsetzen
---
In diesem Projekt werde ich einen Container erstellen auf dem schlussendlich ein voll funktionstüchtigen Mailserver laufen wird den man Zentral über eine Administrations Interface verwalten, monitoren und Anpassen kann. Dabei werde ich in diesem GitHub Repo erklären und beschreiben wie ich diesen Webserver aufgesetzt habe und was die FUnktionen dieses Dienstes sind.

---
# Was ist Mailu?
---
![grafik](logo.png))

Mailu ist ein voll funktionsfähiger Mailserver als Satz von Docker-Images. Man hat mit Mailu die Mögliochkeit, einen leicht zu wartenden und voll ausgestatteten Mailserver aufzusetzen und zur Verfügung zu stellen, ohne proprietäre Software oder nicht damit zusammenhängende Funktionen zu liefern, die oft in populärer Groupware zu finden sind.

Folgende Features sind inbegriffen:

- Standard-E-Mail-Server, IMAP und IMAP+, SMTP und Übermittlung

- Erweiterte E-Mail-Funktionen, Aliase, Domain-Aliase, benutzerdefiniertes Routing

- Webzugriff, mehrere Webmails und Administrationsoberfläche

- Benutzerfunktionen, Aliase, automatische Antwort, automatische Weiterleitung, abgerufene Konten

- Admin-Funktionen, globale Admins, Ankündigungen, Delegierung pro Domain, Kontingente

- Sicherheit, erzwungenes TLS, Letsencrypt!, ausgehendes DKIM, Virenscanner

- Antispam, Auto-Lernen, Greylisting, DMARC und SPF

- Freedom, alle FOSS-Komponenten, kein Tracker enthalten

---
# Umsetzung
---

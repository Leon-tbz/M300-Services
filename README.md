# M300-Services
Modul 300
---
**1. Apache Webserver automatisiert aufsetzen**

Im ersten Schritt werden wir mithilfe von Vagrant, welches schon vor installiert ist, ein Webserver erstellen, welches Automatisiert it einem vorerstelltem Script erstellt wird.

1. Terminal (Bash) öffnen
2. In das M300-Verzeichnis (/M300/vagrant/web) wechseln:

3. $ cd Pfad/zum-M300-Verzeichnis/vagrant/web

4. VM erstellen und starten:

5. $ vagrant up

6. Nachdem der Webserver erstellt wurde und mit dem Port 8080 freigegeben worden ist, kann man jetzt über den Browser mit dem Port 8080 darauf zugreifen.

"http://10.4.43.27/:8080


7. (Optional) $ vagrant destroy -f

Vagrant kann mit diesem Befehl alle VMs erstellen.

---
# Docker Container
---
Container sind eine Virtualisierungstechnik im Computerumfeld, die Anwendungen inklusive ihrer Laufzeitumgebungen voneinander trennt. Im Gegensatz zu einer virtuellen Maschine beinhalten Container kein eigenes Betriebssystem, sondern verwenden das des Systems, auf dem sie installiert sind.

Grund Befehle, um ein Container zu bedienen:

Starten eines Containers im Hintergrund
- $> docker run -djenkins

Starten eines interaktiven Containers
- $> docker run -itubuntubash

Exportiert port von einem Container
- $> docker run -p 80:80 -dnginx

Starten eines benennter Container
- $>docker run --namemydbredis

Neustarten eines gestoppten Container
- $> docker startmydb

Stoppen eines Containers
- $> docker stopmydb

Hinzufügen von metadaten zu einem container
- $> docker run -d \             label=traefik.backend=jenkins jenkins

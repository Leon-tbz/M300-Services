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

---
Dockerhub
---
Docker-Hub ist ein Online-Dienst, der eine Registry und Repositories für Docker-Images beinhaltet. Die Registry teilt sich in einen öffentlichen und einen privaten Teil auf. Im öffentlichen Teil kann jeder Nutzer seine selbst erstellten Images hochladen und anderen Nutzern zur Verfügung stellen.

![grafik](https://user-images.githubusercontent.com/89446419/171114303-bc5bbfc8-1192-4b0f-b1b8-c242b66a5fb3.png)

# Supported tags und respective Dockerfile links

Simple Tags:

20.10.16, 20.10, 20, latest, 20.10.16-alpine3.16
20.10.16-dind, 20.10-dind, 20-dind, dind, 20.10.16-dind-alpine3.16
20.10.16-dind-rootless, 20.10-dind-rootless, 20-dind-rootless, dind-rootless
20.10.16-git, 20.10-git, 20-git, git
20.10.16-windowsservercore-ltsc2022, 20.10-windowsservercore-ltsc2022, 20-windowsservercore-ltsc2022, windowsservercore-ltsc2022
20.10.16-windowsservercore-1809, 20.10-windowsservercore-1809, 20-windowsservercore-1809, windowsservercore-1809

---

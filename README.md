# Geodateninfrastruktur mit Docker"
## OnlineWorkshop auf der FossGIS '21

### Docker
Docker ermöglicht die einfache Bereitstellung von Anwendungen über Container. Container beinhalten alle notwendigen Pakete für die Anwendungen. Die Anwendungen laufen virtualisiert und somit isoliert.

### Einstieg
Starten der GBD Websuite (WebGIS Suite) über Docker.
`docker run -p "3333:80" -d --name gws gbdconsult/gws-server:7.0`
Die Websuite ist erreichbar über `localhost:3333`.

Auflisten alle laufenden Docker-Container:
`docker ps`

Stoppen der Websuite:
`docker stop gws`

Löschen des Containers:
`docker rm gws`

### Docker Compose
Ermöglicht die einfache Konfigurierung unserer (Geodaten)-Infrastruktur in einer (oder mehreren) YAML-Dateien.
Als Beispiel wollen wir unsere Websuite zusammen mit einer PostGIS Datenbank konfigurieren.




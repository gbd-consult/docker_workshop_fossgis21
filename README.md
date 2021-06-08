# Geodateninfrastruktur mit Docker
## OnlineWorkshop auf der FossGIS '21

```
Tristan Kessler
kessler@gbd-consult.de
```


### Docker
Docker ermöglicht die einfache Bereitstellung von Anwendungen über Container. Container beinhalten alle notwendigen Pakete für die Anwendungen. Die Anwendungen laufen virtualisiert und somit isoliert.

### Einstieg
Starten der GBD Websuite (https://gbd-websuite.de/) über Docker.
```bash
docker run -p "3333:80" -d --name gws gbdconsult/gws-server:7.0
```
Die Websuite ist erreichbar über `localhost:3333`.

Auflisten alle laufenden Docker-Container:
```bash
docker ps
```

Stoppen der Websuite:
```bash
docker stop gws
```

Löschen des Containers:
```bash
docker rm gws
```

### Docker Compose
Ermöglicht die einfache Konfigurierung unserer (Geodaten)-Infrastruktur in einer (oder mehreren) YAML-Dateien.
Als Beispiel wollen wir unsere Websuite zusammen mit einer PostGIS Datenbank konfigurieren.




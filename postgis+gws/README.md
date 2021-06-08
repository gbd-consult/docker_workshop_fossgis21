## PostGIS und GWS mit docker-compose

Konfiguration starten:
```bash
docker-compose up -d
```
(-d startet im Hintergrund)

Logdateien anschauen:
```bash
docker-compose logs -f
```

Container neu starten:
```bash
docker-compose restart postgis
```

Konfiguration stoppen:
```bash
docker-compose down
```
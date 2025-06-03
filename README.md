# CRC_ING

## FastAPI + Docker + GitHub Actions + DockerHub

### Opis projektu

Projekt przygotowuje prostą aplikację FastAPI, którą można uruchomić w Dockerze i zdeployować do DockerHub przy użyciu GitHub Actions.

### Technologia
- Python + FastAPI
- Docker
- GitHub Actions
- DockerHub

### Uruchomienie lokalne

Aby uruchomić aplikację lokalnie w Dockerze:

```bash
docker pull sobol2003/ing2025:latest
docker run -p 8000:8000 sobol2003/ing2025:latest
```
Wejdź na: http://localhost:8000/ aby zobaczyć rezultat.

Deployment do DockerHub
Pipeline GitHub Actions został skonfigurowany do:
- budowania obrazu Dockera,
- wysyłania obrazu do DockerHub.

UWAGA:
Obraz dostępny publicznie pod adresem:
https://hub.docker.com/r/sobol2003/ing2025

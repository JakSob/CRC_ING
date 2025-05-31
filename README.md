# CRC_ING

## FastAPI + Docker + GitHub Actions + Azure

### Opis projektu

Projekt przygotowuje prostą aplikację FastAPI, którą można uruchomić w Dockerze i zdeployować do Azure Container Apps przy użyciu GitHub Actions.

### Technologia
- Python + FastAPI
- Docker
- GitHub Actions
- (Docelowo) Azure Container Registry i Azure Container Apps

### Uruchomienie lokalne

Aby uruchomić aplikację lokalnie w Dockerze:

```bash
docker build -t fastapi-app .
docker run -p 8000:8000 fastapi-app
```
Wejdź na: http://localhost:8000/ aby zobaczyć rezultat.

Deployment do Azure
Pipeline GitHub Actions został skonfigurowany do:
- budowania obrazu Dockera,
- wysyłania obrazu do Azure Container Registry (ACR),
- deployowania aplikacji do Azure Container Apps.

UWAGA:
Aktualnie nie posiadam aktywnej subskrypcji Azure, dlatego proces deployowania nie został zakończony pomyślnie.
Wszystkie pliki są przygotowane tak, aby działało to natychmiast po skonfigurowaniu subskrypcji i zasobów w Azure.

# Planificador semanal

Aplicación web estática en HTML, CSS y JavaScript.

## Ejecutar localmente

Abre `index.html` en el navegador.

## Construir y ejecutar con Docker

```bash
docker build -t TU_USUARIO_DOCKER/planificador-semanal:latest .
docker run --rm -p 8080:80 TU_USUARIO_DOCKER/planificador-semanal:latest
```

Abre http://localhost:8080.

## Publicar en Docker Hub

```bash
docker login
docker build -t TU_USUARIO_DOCKER/planificador-semanal:latest .
docker push TU_USUARIO_DOCKER/planificador-semanal:latest
```

Sustituye `TU_USUARIO_DOCKER` por tu usuario de Docker Hub.

## Publicar en GitHub

Crea un repositorio vacío en https://github.com/new y luego ejecuta desde esta carpeta:

```bash
git init
git add .
git commit -m "Publicar planificador semanal"
git branch -M main
git remote add origin https://github.com/TU_USUARIO_GITHUB/planificador-semanal.git
git push -u origin main
```

## Nota sobre cuentas y datos

La aplicación guarda tareas y cuentas en `localStorage` del navegador. El inicio de sesión
es local y no constituye autenticación segura para producción; no uses contraseñas reales
ni datos sensibles. Para cuentas compartidas entre dispositivos hace falta un backend.

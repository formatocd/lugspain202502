# Meetup Liferay User Group Spain febrero 2025

## _Con un API y con paciencia, Liferay pierde la cabeza_
Está charla tendrá formato taller y nos permitirá probar como conectamos sistemas externos con arquitecturas distintas al API Headless de Liferay

## Requisitos para el taller
- [Docker](https://www.docker.com/)
- [Instalador de Laravel](https://laravel.com/docs/11.x/installation#installing-php)
- [Cliente Git](https://git-scm.com/downloads)
- [Node.js y NPM](https://nodejs.org/es) (o con [NVM](https://github.com/coreybutler/nvm-windows))

## Ficheros para el taller
[Ver ficheros](https://gist.github.com/formatocd/881eb95166e52c604a5bbe95fc995e0b)

## Preparación de entornos
### Laravel
Descargamos un proyecto nuevo de Laravel
```bash
laravel new nombre-proyecto
```
Entramos en el directorio creado, añadimos TailwindCSS y compilamos.
```bash
cd nombre-proyecto
npm install tailwindcss @tailwindcss/vite
npm install && npm run build
```
Para arrancar el servidor ejecutamos:
```bash
composer run dev
```
### Liferay
Descargar el proyecto Liferay Docker:
```bash
git clone https://github.com/formatocd/liferay-docker.git
```
Lanzar el contenedor:
```bash
cd liferay-docker\postgresql
docker compose up -d
```
### Acceso a los entornos
- ***Liferay***: http://localhost:18080
- ***Laravel***: http://localhost:8000


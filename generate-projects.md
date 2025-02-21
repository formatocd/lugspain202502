[Inicio](./lugspain202502) / Generacíon de proyectos

# Generacíon de proyectos

## Laravel

### Crear el proyecto

Ejecutar el comando:

```bash
laravel new project-name
```

El programa de instalación te hará algunas preguntas. Basta con que pulses Enter en todas para proseguir con los valores por defecto.

### Inicializar el proyecto

Una vez se haya generado el proyecto, accedemos al directorio `project-name` e inicializamos el proyecto:

```bash
cd project-name
npm install
npm run build
```

### Arrancar el servidor

Para arrancar el proyecto ejecuta el comando:

```bash
composer run dev
```

El proceso se quedará imprimiendo la traza en el terminal. El proyecto estará accesible desde el navegador en http://localhost:8000

## Liferay
> [!IMPORTANT]
> Requiere que Docker Desktop este arrancado

### Descargar el proyecto
```bash
git clone https://github.com/formatocd/liferay-docker.git
```
### Inicializar el contenedor
```bash
cd liferay-docker
docker compose up -d
```

Cuando termine de arrancar el contenedor completamente, el portal Liferay estará accesible desde el navegador en http://localhost:18080



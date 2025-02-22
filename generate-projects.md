[Inicio](/lugspain202502) / Generacíon de proyectos

# Generacíon de proyectos

## Laravel

### Crear el proyecto

Ejecutar el comando:

```bash
laravel new project-name
```

El programa de instalación te hará algunas preguntas. Basta con que pulses Enter en todas para proseguir con los valores por defecto.

### Inicializar el proyecto

Una vez se haya generado el proyecto, accedemos al directorio `project-name`, añadimos la dependencia de TailwindCSS e inicializamos el proyecto:

```bash
cd project-name
npm install tailwindcss @tailwindcss/vite
npm install
npm run build
```

### Arrancar el servidor

Para arrancar el proyecto ejecuta el comando:

```bash
composer run dev
```

El proceso se quedará imprimiendo la traza en el terminal. El proyecto estará accesible desde el navegador en http://localhost:8000

### Error _failed to listen_
Si al ejecutar `composer run dev` te aparece una traza como esta:
```
[server]   Failed to listen on 127.0.0.1:8001 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8002 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8003 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8004 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8005 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8006 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8007 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8008 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8009 (reason: ?)
[server]   Failed to listen on 127.0.0.1:8010 (reason: ?)
[server] php artisan serve exited with code 1
```
Ejecuta el comando
```bash
php --ini
```
Te devolverá algo así:
```
Configuration File (php.ini) Path:
Loaded Configuration File:         C:\Users\Carlos\.config\herd-lite\bin\php.ini
Scan for additional .ini files in: (none)
Additional .ini files parsed:      (none)
```

Edita el fichero `php.ini` que te indica y edita la propiedad `variables_order` para que quede así:
```ini
variables_order = "GPCS"
```


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



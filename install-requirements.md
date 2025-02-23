> [Inicio](./) / Instalación de requisitos

# Instalación de requisitos
## NVM (Node.js)
### Windows
Descargamos el instalador de <a href="https://github.com/coreybutler/nvm-windows/releases/download/1.2.2/nvm-setup.exe" target="_blank">NVM for Windows</a> y lo ejecutamos.
> **CONSEJO**
> 
> Por defecto la instalación abre la ventana de PowerShell al terminar. Si no funcionara el comando `nvm`, cerrar todas las ventanas de PS y volver a abrir una nueva.
### Linux & Mac
Sigue las <a href="https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating" target="_blank">instrucciones</a> en repositorio oficial.

### Instalar Node y npm
Ejecuta los siguientes comandos:
```bash
nvm install 22
nvm use 22
```
#### Error de ejecución de scripts en Windows
Después de instalar **NVM**, ejecuta el comando:
```bash
npm -v
```

Si el comando falla y te da el mensaje `No se puede cargar el archivo C:\nvm4w\nodejs\npm.ps1 porque la ejecución de scripts está deshabilitada en este sistema`, ejecuta el siguiente comando en una **terminal PowerShell con permiso de Administrador**:
```bash
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser 
```

## Composer, PHP, Laravel Installer
### Windows (Powershell)
> **IMPORTANTE**
> 
> Requiere ejecutar **Powershell en modo Administrador**
```bash
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://php.new/install/windows/8.4'))
```
### macOS
```bash
/bin/bash -c "$(curl -fsSL https://php.new/install/mac/8.4)"
```
### Linux
```bash
/bin/bash -c "$(curl -fsSL https://php.new/install/linux/8.4)"
```
## Docker Desktop
> **CONSEJO**
>
> Sólo necesario si se va a usar Liferay portal en modo contenedor

<a href="https://www.docker.com/products/docker-desktop/" target="_blank">Descarga</a> e instala la versión de Docker correspondiente a tu sistema operativo


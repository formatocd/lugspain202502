[Inicio](./lugspain202502) / Instalación de requisitos



# Instalación de requisitos
## NVM (Node.js)
### Windows
Descargamos el instalador de [NVM for Windows](https://github.com/coreybutler/nvm-windows/releases/download/1.2.2/nvm-setup.exe) y lo ejecutamos.
> [!TIP]
> Por defecto la instalación abre la ventana de PowerShell al terminar. Si no funcionara el comando `nvm`, cerrar todas las ventanas de PS y volver a abrir una nueva.
### Linux & Mac
Sigue las [instrucciones](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating) en repositorio oficial.

### Instalar Node y npm
Ejecuta los siguientes comandos:
```bash
nvm install 22
nvm use 22
```
#### Error de ejecución de scripts en Windows
Si después de instalar `node` y `npm`, al ejecutar cualquier comando de los dos falla y te sale el mensaje `No se puede cargar el archivo C:\nvm4w\nodejs\npm.ps1 porque la ejecución de scripts está deshabilitada en este sistema`, ejecuta el siguinete comando en PS con permiso de Administrador:
```bash
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser 
```

## Vite
> [!IMPORTANT]
> Requiere tener instalado **npm**

Ejecuta este comando:
```bash
npm install -D vite
```

## Composer, PHP, Laravel Installer
### Windows (Powershell)
> [!IMPORTANT]
> Requiere ejecutar Powershell en modo Administrador
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


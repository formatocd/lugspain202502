[Inicio](./lugspain202502) / Instalación de requisitos

# Instalación de requisitos
## NVM (Node.js)
### Windows
Descargamos el instalador de [NVM for Windows](https://objects.githubusercontent.com/github-production-release-asset-2e65be/24268127/391aac33-6576-461a-9740-16767aa1db06?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=releaseassetproduction%2F20250221%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250221T184541Z&X-Amz-Expires=300&X-Amz-Signature=659ea7c6e359c926029868413b34ecc6822718349f8216e13a01cd5a2c5a6c47&X-Amz-SignedHeaders=host&response-content-disposition=attachment%3B%20filename%3Dnvm-setup.exe&response-content-type=application%2Foctet-stream) y lo ejecutamos.
### Linux & Mac
Sigue las [instrucciones](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating) en repositorio oficial.

### Instalar Node y npm
Ejecuta los siguientes comandos:
```bash
nvm install 22
nvm use 22
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


### ¿Porqué Vagrant?

Vagrant maneja los procesos de creacion de una maquina virtual basado en tus definiciones, y usa herramientas de automatización como Ansible y Puppet para provisionar la customizacion de la maquina - instalando paquetes, reuniendo información, realizando tareas, etc.

+++

## Ventajas

- Potabilidad
- Utilizar herramientas de provisionamiento
- Encapsulamiento
- Limitanción recursos
- Kernel

---

## Tecnologías necesarias

1. Powershell
2. Openssh
3. Virtualbox
4. Vagrant

---

### Intalar

## Powershell

A. Descargar e installar powershell

https://github.com/PowerShell/PowerShell/releases/tag/v6.0.0-beta.7

+++

## Install openssh

B. Iniciar cmd como admnistrador

1. Instalar chocolatey

```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

2. Instalar openssh
```
choco install openssh
```

3. Recargar el ambiente
```
refreshenv
```

+++

## Install virtualbox

Instalar virtualbox

https://www.virtualbox.org/wiki/Downloads

+++

## Vagrant

Instalar Vagrant

https://www.vagrantup.com/downloads.html

---

### Iniciar maquina virtual

1. Crear un directorio de trabajo
2. Iniciar powershell y entrar a la ruta de trabajo
3. Clonar el repo o descargarlo directamente
```
git clone https://github.com/Tinker-Ware/vagrant-tutorial.git
```
3. Entrar al folder
```
vagrant-tutorial.git
```
4. Ejecutar
```
vagrant up
```

---

## Install .NET

1. Agregar el .NET product feed

```
sudo apt-get update
```

```
sudo apt-get install curl libunwind8 gettext apt-transport-https
```

```
curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
```

```
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
```

```
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/microsoft-debian-jessie-prod jessie main" > /etc/apt/sources.list.d/dotnetdev.list'
```

+++

2. Instalar .NET Core SDK

```
sudo apt-get update
```

```
sudo apt-get install dotnet-sdk-2.0.0
```

+++

3. Crear un proyecto

```
dotnet new console -o newProyect
```

```
cd newProyect
```

```
dotnet run
```

---

## Comandos de Vagrant

1. Vagrant ssh. Entrar mediante ssh a la máquina virtual.
2. Vagrant up. Iniciar la máquina virtual.
3. Vagrant status. Ver el estatus de la máquina virtual.
4. Vagrant halt. Apagar máquina virtual.
5. Vagrant destroy. Destruir máquina virtual.
6. Vagrant reload. Recargar coniguración.

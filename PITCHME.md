### ¿Porqué Vagrant?

Vagrant maneja los procesos de creacion de una maquina virtual basado en tus definiciones, y usa herramientas de automatización como Ansible y Puppet para provisionar la customizacion de la maquina - instalando paquetes, reuniendo información, realizando tareas, etc.

Corriendo unicamente ***vagrant up***, una maquina virtual será preparada de acuerdo a la confinguración especificada en el archivo de configuración.

---

### Intalar

## Powershell

A. Descargar e installar powershell

https://github.com/PowerShell/PowerShell/releases/tag/v6.0.0-beta.7

+++

## Install openssh

B. Iniciar cmd como admnistrador y correr los siguientes comandos

1. Para instalar chocolatey correer el siguiente comando:

```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"
```

2. Para instalar openssh correer el siguiente comando:
```choco install openssh```

3. Para recargar el ambiente correr el siguiente comando:
```refreshenv```

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
3. Clonar el repo con el comando `git clone https://github.com/Tinker-Ware/vagrant-tutorial.git` o descargarlo directamente si no se tiene git instalado.
3. Entrar al folder `vagrant-tutorial.git`
4. Ejecutar el comando `vagrant up`

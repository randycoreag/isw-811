# Workshop 01

![Virtualizacion](./images/header.png)

## Orden de Instalacion de Softwares

- Virtual Box
- Extension
- Vagrant
- Notepad ++
- Git


## Comandos para Sobrevivir en Bash Linux

- `pwd`: Imprimir el directo actual
- `cs`: Cambiar directorio
- `mkdir`: Crear directorio
- `touch`: Crear un archivo vacio
- `ls`: Listar el directorio actual
-  `ls - la`: Listar el directorio actual, incluyendo archivos ocultos

## Aprovisionar Maquina Debian Bookworm

- `vagrant init debian/bookworm64:` lo utilizamos para descargar la imagen y version correspondiente de Debian
- `vagrant up:` se utiliza para realizar la descarga e instalacion asi como para iniciar la maquina
- `vagrant status:` se utiliza para verificar el estado de la maquina
- `vagrant ssh:` lo utilizamos para conectarnos a la maquina virtual
- `vagrant hatl:` se utilizar para desconectarse y apagar la maquina

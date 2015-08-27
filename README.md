# datos-spark-lab
## Spark Lab para Organizacion de Datos 75.06

### Instalacion: Pre Requisitos

Para poder utilizar la VM debe tener instalado [VirtualBox](https://www.virtualbox.org/) y [Vagrant](https://www.vagrantup.com/).

* Video de instalacion de [VirtualBox](https://www.virtualbox.org/) en linux: [https://www.youtube.com/watch?v=1_4USzcKx6g](https://www.youtube.com/watch?v=1_4USzcKx6g)
* Guia de instalación de [Vagrant](https://www.vagrantup.com/): [https://docs.vagrantup.com/v2/installation/index.html](https://docs.vagrantup.com/v2/installation/index.html)
* Video de instalacion de [Vagrant](https://www.vagrantup.com/) en linux [https://www.youtube.com/watch?v=f2cufy6wRfA](https://www.youtube.com/watch?v=f2cufy6wRfA)

## Trabajando con la VM

1. Para iniciar la VM, desde la linea de comandos ejecutar el comando `vagrant up`.
2. Para cerrar la VM, desde la linea de comandos ejecutar. `vagrant halt`. Es recomendable bajar la VM antes de reiniciar o apagar tu computadora.
3. Para destruir la VM, desde la linea de comandos ejectura el comando `vagrant destroy`. Se puede nuevamente crear la misma con el comando "vagrant up"
4. Una vez que la VM esta funcionado se puede acceder a IPython Notebook abriendo un browser http://127.0.0.1:8001/
5. para probar otras o ver su contenido, se pueden conectar via ssh usando `vagrant ssh` 

## Disponibilizar archivos en la VM
Todo archivo que sea guardado en este directorio (donde se encuentra el Vagrantfile, sera visible en la VM bajo el directorio `/vagrant` y accesible desde IPython Notebook usando el fullpath.

## Ampliando la VM
Se puede utilizar el archivo bootstrap.sh para agregar nuevas librerias de python y otras necesidades que se tengan en la VM para amplicar su funcionamiento.
En este caso se utiliza para la instalacion de numpy y matplotlib que se usan para los ejemplos notebooks: 002 y 003
Este script se ejecuta durante el provisioning de la maquina al ejecutar `vagrant up` o una vez que la maquina esta funcionando con `vagrant provision`

### Agradecimientos
El trabajo de este lab esta basado en el de https://github.com/spark-mooc/mooc-setup cuyo material fue de gran ayuda para elaborar el lab.

# Instalación de R en el sistema operativo Ubuntu

El procedimiento que se describe a continuación está basado en el tutorial [How To Install R on Ubuntu 16.04 | Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-16-04-2). Instala la versión más reciente que esté disponible en los repositorios de [R](https://www.r-project.org/). Debe ser ejecutado por un usuario con derechos de ```sudo```.

El procedimiento fue probado en una instalación de [Ubuntu 16.04 LTS (Xenial Xerus)](http://releases.ubuntu.com/16.04/).

```terminal
# Descarga de las llaves de autenticación del repositorio con los paquetes de R
$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9

# Adición del repositorio con los paquetes de R
$ sudo add-apt-repository 'deb [arch=amd64,i386] https://cran.rstudio.com/bin/linux/ubuntu xenial/'

# Actualización de los repositorios
$ sudo apt-get update

# Instalación de R
$ sudo apt-get install r-base

# Inicio de R (en modo superusuario para, por ejemplo, instalar paquetes)
$ sudo -i R
```

Ejemplo de instalación de paquetes
```terminal
> install.packages('txtplot')
```

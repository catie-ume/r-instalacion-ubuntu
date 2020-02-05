# Instalación de R en el sistema operativo Ubuntu

El procedimiento que se describe a continuación está basado en el tutorial [How To Install R on Ubuntu 16.04 | Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-r-on-ubuntu-16-04-2).

```terminal
# Descarga de las llaves de autenticación
$ sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9

# Adición del repositorio
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

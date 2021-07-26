#Descargamos UBUNTU 
FROM ubuntu 

##Actualizamos el sistema
RUN apt-get update 

##En algunas versiones de Linux es necesario configurar una variable para el TIMEZONE 
ENV TZ=Europe/Madrid 

##Luego creamos un fichero llamado /etc/timezone para configurar 
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone 

##Instalamos PYTHON
RUN apt-get install -y python

##Instalamos PYTHON
RUN apt-get install -y git


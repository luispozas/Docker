FROM centos 

#Hacemos el update y la instalacion
RUN yum -y update 
RUN yum -y install java-1.8.0-openjdk.x86_64 && yum -y install wget && yum -y install lsof

#Seguimos los pasos para la instalacion de solr en la documentacion
WORKDIR /opt 
RUN wget https://downloads.apache.org/lucene/solr/8.9.0/solr-8.9.0.tgz 
RUN tar xzf solr-8.9.0.tgz 

#Ponemos el puerto 
EXPOSE 8983

#Iniciamos solr en modo -f : FOREGROUND 
CMD ["/opt/solr-8.9.0/bin/solr","start","-force","-f"]


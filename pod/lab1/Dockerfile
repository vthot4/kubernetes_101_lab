FROM ubuntu:18.04
MAINTAINER vteteam "vteteam@versia.com"
RUN apt-get update -y
##Instalamos nginx
RUN apt-get install -y nginx
##Creamos un fichero index.html en el directorio por defecto de nginx
RUN echo 'Primer POD con yaml' > /usr/share/nginx/www/index.html
##Arrancamos NGINX a través de ENTRYPOINT
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
EXPOSE 80
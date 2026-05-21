FROM ubuntu:latest 
LABEL "Authur" = "Girish"
LABEL "Project" = "nano"
ENV DEBIAN_FORNTEND = noninteractive
RUN apt update && apt  install git -y
RUN apt install apache2 -y 
CMD ["/usr/sbin/apache2ctl", "-D" , "FOREGROUND"]
EXPOSE 80
WORKDIR /Var/www/html 
VOLUME /var/log/apache2
ADD nano.tar.gz /var/www/html
#COPY nano.tar.gz /Var/www/html 



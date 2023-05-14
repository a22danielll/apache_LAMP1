FROM debian
RUN apt-get update && apt-get install -y apache2 php libapache2-mod-php php-zip php-xml php-curl php-gd php-mysql php-intl php-mbstring
RUN a2enmod ssl
RUN a2enmod rewrite
EXPOSE 80
EXPOSE 443
WORKDIR /app

CMD chmod 777 /app/* && apachectl -D FOREGROUND
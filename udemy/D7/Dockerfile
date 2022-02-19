ARG CODE_VERSION=16.04
FROM ubuntu:${CODE_VERSION}
LABEL Creator: "Cerulean Canvas"

RUN apt-get update && apt-get install -y apache2 && apt-get clean && rm -rf /var/lib/apt/lists/*

# environment variables
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2

# listening port
EXPOSE 80

CMD ["/usr/sbin/apache2","-D","FOREGROUND"]

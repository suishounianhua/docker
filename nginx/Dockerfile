FROM ubuntu:latest
# Identify the maintainer of an image
MAINTAINER peterpang "10846295@qq.com"
# Update the image to the latest packages
RUN apt-get update && apt-get upgrade -y
# Install NGINX to test.
RUN apt-get install nginx -y

# Expose port 80
EXPOSE 80

USER www-data

VOLUME /home/docker/web

WORKDIR /home/web
#
# Last is the actual command to start up NGINX within our Container
CMD ["nginx", "-g", "daemon off;"]

FROM nginx:latest

# Instalar Maven y Docker
RUN apt-get update && apt-get install -y maven docker.io
RUN mvn -f hola-mundo/pom.xml clean package
# Copia tu archivo HTML
COPY index.html /usr/share/nginx/html/index.html

# Exponer el puerto 80
EXPOSE 80

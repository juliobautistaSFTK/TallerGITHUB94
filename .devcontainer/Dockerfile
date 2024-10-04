FROM nginx:latest

# Instalar Maven y Docker
RUN apt-get update && apt-get install -y maven docker.io && systemctl enable docker && systemctl start docker

# Copia tu archivo HTML
COPY index.html /usr/share/nginx/html/index.html

# Exponer el puerto 80
EXPOSE 80

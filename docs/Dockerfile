FROM nginx:latest
ENV APP_VERSION=1.0.0
ENV OWNER=YourName
RUN apt-get update && apt-get install -y curl vim
COPY index.html /usr/share/nginx/html/index.html
HEALTHCHECK --interval=30s --timeout=3s \\
  CMD curl -f http://localhost/ || exit 1

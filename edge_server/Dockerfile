FROM alpine:latest
LABEL org.opencontainers.image.authors="divyenduJoshi"
RUN apk update && apk add nginx 
COPY config/nginx.conf /etc/nginx/
COPY web_content/ /var/www
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

FROM nginx:alpine

EXPOSE 80
EXPOSE 443

RUN apk add ca-certificates 
COPY ./conf /etc/nginx/conf.d
COPY ./ssl /ssl
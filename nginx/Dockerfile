FROM nginx:1.25-alpine

RUN apk add --no-cache apache2-utils libxml2 libxslt curl git \
  && mkdir -p /etc/nginx/modsec /etc/nginx/certs

COPY default.conf /etc/nginx/conf.d/default.conf
COPY waf/modsecurity.conf /etc/nginx/modsec/modsecurity.conf

RUN sed -i '/http {/a \    server_tokens off;' /etc/nginx/nginx.conf

RUN adduser -D -g 'www' nginxuser && \
  chown -R nginxuser:nginxuser /var/cache/nginx /var/run /var/log/nginx /etc/nginx

USER nginxuser

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]

FROM nginx:1.25-alpine

# RUN rm -f /etc/nginx/conf.d/default.conf

# COPY default.conf /etc/nginx/conf.d/default.conf

# RUN mkdir -p /var/cache/nginx/client_temp && \
#   chown -R nginx:nginx /var/cache/nginx && \
#   chmod -R 755 /var/cache/nginx


EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

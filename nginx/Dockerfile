FROM nginx:1.25-alpine

# Supprimer la config par défaut si existante
# RUN rm -f /etc/nginx/conf.d/default.conf

# Copie de ta configuration personnalisée
# COPY default.conf /etc/nginx/conf.d/default.conf

# Correction des permissions pour éviter les erreurs
# RUN mkdir -p /var/cache/nginx/client_temp && \
#   chown -R nginx:nginx /var/cache/nginx && \
#   chmod -R 755 /var/cache/nginx

# Désactive la directive "user nginx;" si tu l'as dans nginx.conf
# Sinon, NGINX tentera de drop les privilèges (et échouera si pas root)
# Alternativement, si tu veux la laisser, assure-toi d’exécuter en root.

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]

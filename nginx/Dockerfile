FROM dnadas98/freeroam:frontend_angular as build_frontend

FROM nginx:latest

# frontend
COPY --from=build_frontend /home/app/dist /usr/share/nginx/html/frontend
RUN chown -R nginx:nginx /usr/share/nginx/html/frontend
RUN chmod -R 755 /usr/share/nginx/html/frontend

# ssl
COPY --chmod=600 --chown=nginx:nginx  ssl/fake-ssl-cert /etc/nginx/ssl/freeroam.crt
COPY --chmod=600 --chown=nginx:nginx  ssl/fake-ssl-key /etc/nginx/ssl/freeroam.key

# config
COPY --chown=nginx:nginx --chmod=644 nginx.conf /etc/nginx/conf.d/default.conf

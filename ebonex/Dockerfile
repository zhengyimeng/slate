FROM nginx:1.14
RUN mkdir -p /broker/www
EXPOSE 80/tcp
EXPOSE 443/tcp
COPY build /broker/www
COPY ./nginx.conf /etc/nginx/conf.d/default.conf
RUN chown -R nginx:nginx /broker

FROM nginx:1.24
RUN rm -rf /etc/nginx/conf.d/default.conf
RUN rm -rf /usr/share/nginx/html/
RUN rm -rf /etc/nginx/nginx.conf
COPY nginx.conf /etc/nginx/nginx.conf
COPY static /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
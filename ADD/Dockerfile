FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/Devi-036/SQL_Data_Analytics/refs/heads/main/scripts/00_init_database.sql /usr/share/nginx/html/index.html 
RUN chmod +r /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]

FROM almalinux:9
LABEL course="devops" \
      duration="120 HRS"
EXPOSE 80            
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# COPY google/ /usr/share/nginx/html/
ADD https://raw.githubusercontent.com/daws-84s/notes/refs/heads/main/session-50.txt /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]

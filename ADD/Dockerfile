FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index,html
ADD https://www.dpreview.com/samples/3925134721/fujifilm-x-a3-sample-gallery /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
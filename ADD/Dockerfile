FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index,html
ADD https://gist.github.com/lillylangtree/b55828fa05ed3470d352 /usr/share/nginx/html/index.html
#So we download directly to the internet /usr/share/nginx/html/index.html path does not have the permissions to read so that we have to provided or else we are getting 403 forbidden error
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
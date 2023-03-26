FROM nginx:alpine
COPY nginx.conf /etc/nginx/nginx.conf
COPY tls/. /etc/nginx/ssl
CMD ["nginx", "-g", "daemon off;"]
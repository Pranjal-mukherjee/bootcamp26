FROM nginx:alpine
COPY nginx.conf /etc/nginx/conf.d/default.conf
RUN rm -rf /usr/share/nginx/html/*
COPY dist/ /usr/share/nginx/html
EXPOSE 80
ENTRYPOINT ["nginx","-g","daemon off;"]

# ENTRYPOINT ["nginx","-g","daemon off;"]:
# This instruction sets the 
# command that will be executed when the container starts. It runs
#  NGINX with the provided arguments -g "daemon off;", which tells 
#  NGINX to run in the foreground. This is important for Docker containers,
#  as they need a foreground process to keep the container running.
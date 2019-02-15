FROM nginx:stable-alpine

LABEL maintainer="Timothy J. Scott"

# main configuration file
RUN rm /etc/nginx/nginx.conf
COPY ./nginx.conf /etc/nginx/

# any additional configuration files
RUN rm /etc/nginx/conf.d/default.conf
COPY ./demo_app_service.conf /etc/nginx/conf.d/

# mount folders with static content
ADD ./data /data/
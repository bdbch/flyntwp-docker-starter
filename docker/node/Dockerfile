FROM node:14 as node

COPY wp-content /wp-content
WORKDIR /wp-content/themes/flynt

RUN apt install python -y

EXPOSE 3000

CMD ["tail", "-f", "/dev/null"]
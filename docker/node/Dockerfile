FROM --platform=linux/amd64 node:14 as node

WORKDIR /theme

COPY /wp-content/themes/flynt /theme

RUN apt install python -y

EXPOSE 3000

CMD ["tail", "-f", "/dev/null"]
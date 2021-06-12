FROM node:14 as node

COPY /wp-content/themes/flynt /theme
WORKDIR /theme

RUN apt install python -y

EXPOSE 3000

CMD ["tail", "-f", "/dev/null"]
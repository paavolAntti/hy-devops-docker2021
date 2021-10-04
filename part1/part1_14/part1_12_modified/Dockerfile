FROM ubuntu:18.04

RUN apt-get update && apt-get install -y curl

EXPOSE 5000

WORKDIR /usr/src/app

COPY /example-frontend .

ENV REACT_APP_BACKEND_URL=http://localhost:8080/

RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -

RUN apt install -y nodejs

RUN npm install -g serve

RUN npm install

RUN npm run build


CMD [ "serve", "-s", "-l", "5000", "build" ]

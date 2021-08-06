FROM ubuntu:18.04

copy input.sh .

RUN chmod +x input.sh

RUN apt-get -y update; apt-get -y upgrade; apt-get -y install curl

CMD ./input.sh
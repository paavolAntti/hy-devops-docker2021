FROM golang:1.16

EXPOSE 8080

WORKDIR /usr/src/app

COPY /example-backend .

ENV REQUEST_ORIGIN=http://127.0.0.1:5000

RUN go build

CMD ["./server"]
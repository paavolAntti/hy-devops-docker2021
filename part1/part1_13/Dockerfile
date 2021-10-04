FROM golang

EXPOSE 8080

WORKDIR /usr/src/app

COPY /example-backend .

RUN go build

CMD ["./server"]
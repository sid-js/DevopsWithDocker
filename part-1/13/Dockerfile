FROM golang:1.16

WORKDIR /usr/src/app

EXPOSE 8080

COPY . .

RUN go build

RUN go test ./...

ENV REQUEST_ORIGIN=http://localhost:8080/ping

CMD ["./server"]
FROM golang:1.16.15

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

ENV REQUEST_ORIGIN=http://localhost

RUN go build

RUN go test ./...

CMD ./server

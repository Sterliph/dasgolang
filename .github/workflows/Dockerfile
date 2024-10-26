FROM golang:1.23.2-alpine3.20

WORKDIR /app

COPY . /app

RUN go get .

RUN  go test ./...

RUN go build ./main.go

EXPOSE 8080

CMD ['/app/main']
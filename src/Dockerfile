FROM golang:latest

RUN mkdir /opt/userapi

COPY *.go /opt/userapi/

WORKDIR /opt/userapi

RUN go get github.com/go-sql-driver/mysql

RUN go get github.com/gorilla/mux

RUN go build -o main.go .

CMD ["/opt/userapi/main.go"]
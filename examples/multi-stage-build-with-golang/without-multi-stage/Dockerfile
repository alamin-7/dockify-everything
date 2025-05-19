FROM golang:1.21 

WORKDIR /test

COPY server.go .

RUN go build -o app server.go

EXPOSE 8080

CMD [ "./app" ]
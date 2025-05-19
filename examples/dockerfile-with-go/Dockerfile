FROM golang:1.21

WORKDIR /app

COPY first.go . 

RUN go build -o app first.go

CMD [ "./app" ]
# stage-1: Build

FROM golang:1.21 as builder

WORKDIR /test

COPY  server.go .

#  disable c language bindings in go
ENV CGO_ENABLED=0

# Sets the target operating system to Linux for the compiled binary.
ENV GOOS=linux

# Disable Go modules (optional for simple apps)
ENV GO111MODULE=off

RUN go build -o app server.go

# stage-2: Run

FROM scratch

WORKDIR /test

COPY --from=builder /test/app .

EXPOSE 8080

CMD [ "./app" ]
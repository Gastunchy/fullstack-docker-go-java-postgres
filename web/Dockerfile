FROM golang:alpine as builder

WORKDIR /build

COPY . .

RUN go build dispatcher.go

FROM alpine:edge

WORKDIR /app

EXPOSE 80

COPY --from=builder /build/ .

CMD ./dispatcher
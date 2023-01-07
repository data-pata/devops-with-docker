# Exercise 1.13: Hello, backend!

FROM golang:1.16

WORKDIR /usr/src/app



# pre-copy/cache go.mod for pre-downloading dependencies and only redownloading them in subsequent builds if they change
COPY go.mod go.sum ./
RUN go mod download && go mod verify

COPY . .

ENV PORT=8080 \
    REQUEST_ORIGIN=http://localhost:5000

RUN go build

EXPOSE 8080

CMD ["./server"]

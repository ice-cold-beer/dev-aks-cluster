# Use a smaller image
FROM golang:1.21rc4-alpine3.18

WORKDIR /go-hello-world

COPY go.mod go.sum ./
RUN go mod download

# Add stages to the build

COPY . .

CMD ["go", "run", "main.go"]

EXPOSE 8080
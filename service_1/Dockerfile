FROM golang:1.21-alpine

WORKDIR /app
COPY . .

# Automatically init go.mod if missing
RUN go mod init service1 || true

RUN go build -o main .

EXPOSE 8080
CMD ["./main"]
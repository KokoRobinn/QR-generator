FROM golang:1.25

WORKDIR /usr/src/app

COPY go.mod ./
RUN go mod tidy
RUN go mod download

COPY . .
EXPOSE 1010
RUN go build -v -o /usr/local/bin/app ./...

CMD ["app"]

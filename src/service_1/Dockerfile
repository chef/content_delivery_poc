FROM golang:1.17.5-alpine

WORKDIR /app
RUN go mod init content-delivery-system/service_1
RUN go mod tidy
RUN go get github.com/gin-gonic/gin
COPY ./main.go .

CMD ["go", "run", "."]
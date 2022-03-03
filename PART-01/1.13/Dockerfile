FROM golang:1.16

WORKDIR /usr/src/app
COPY ./PART-01/1.13/example-backend .

RUN go build

EXPOSE 8080

CMD ["./server"]


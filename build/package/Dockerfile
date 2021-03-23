FROM golang:1.10 AS build
WORKDIR /go/src
COPY pkg/generated/server ./github.com/sbnarra/alarming-api/pkg/generated/server
COPY cmd/main.go .

ENV CGO_ENABLED=0
RUN go get -d -v ./...

RUN go build -a -installsuffix cgo -o alarming .

FROM scratch AS runtime
COPY --from=build /go/src/alarming ./
EXPOSE 8080/tcp
ENTRYPOINT ["./alarming"]

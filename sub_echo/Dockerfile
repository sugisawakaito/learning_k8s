FROM golang:1.21.4-bullseye as build

WORKDIR /app

COPY go.mod go.sum ./
RUN go mod download

COPY . .
RUN go build -trimpath -ldflags "-w -s" -o app

FROM debian:bullseye-slim as deploy

RUN apt-get update

COPY --from=build /app/app .

EXPOSE 8050

CMD ["./app"]

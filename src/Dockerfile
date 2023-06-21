## Build
FROM golang:1.18 AS build

WORKDIR /app

COPY go.* ./
COPY *.go ./
RUN go mod download
RUN go build -o /employees-service

## Deploy
FROM gcr.io/distroless/base-debian10

WORKDIR /

COPY --from=build /employees-service /employees-service

EXPOSE 8080

USER nonroot:nonroot

ENTRYPOINT ["/employees-service"]
# Golang gRPC Protobuf REST

Sekedar proyek belajar Golang gRPC Protobuf dan REST

## Build RPC dan REST Server

```bash
cd cmd/server
go build .
```

## Build RPC dan REST Client

```bash
cd cmd/client/grpc
go build .

cd cmd/client/rest
go build .
```

## Run Server

```bash
./server -grpc-port=9090 -http-port=8080 -db-host=localhost:3306 -db-user=root -db-password=aden -db-schema=go_todo -log-level=-1 -log-time-format=2006-01-02T15:04:05.999999999Z07:00

```

## Run REST Client 

```bash
./rest -server=http://localhost:8080
```

## Run RPC Client 

```bash
./grpc -server=http://localhost:9090
```

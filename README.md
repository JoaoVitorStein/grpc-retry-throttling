# grpc-retry-throttling
Repository to exemplify that retry throttling for gRPC is not working as expected.
Even configuring the retry throttling, the retries are not being throttled after failures with RPCs.

## How to run
1. Build
```shell
./gradlew build
```

2. Run the server
```shell
java -cp  ./build/libs/grpc-retry-throttling-1.0-SNAPSHOT-all.jar  org.example.RetryingHelloWorldServer
```

2. Run the client
```shell
java -cp  ./build/libs/grpc-retry-throttling-1.0-SNAPSHOT-all.jar  org.example.RetryingHelloWorldClient
```
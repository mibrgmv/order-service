# Order Service
## Project structure
- [API Gateway](https://github.com/mibrgmv/order-service-gateway/)
- [Order Creation Service](https://github.com/mibrgmv/order-creation-service/)
- [Order Processing Service](https://github.com/mibrgmv/order-processing-service/)

## Cheatsheets
github auth for pushing docker images
```shell
echo "access token" | docker login ghcr.io -u <github-username> --password-stdin
```
publish a docker image to github
```shell
docker build -t <service-name>:latest -f path/to/Dockerfile .

docker tag <service-name>:latest ghcr.io/<github-username>/<service-name>:latest

docker push ghcr.io/<github-username>/<service-name>:latest
```
send requests to gRPC service directly with grpcui
```shell
grpcui -plaintext <host>:<port>
```

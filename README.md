# go-grpc-graphql
Go (1.15.x) Google GRPC, GraphQL and Jaegar distributed tracing injection (including Dockerfile)


### Compiling the microservice {account, order, order_catalog}.proto files

#### For the account service, change into the services/account directory where the account.proto file is
`protoc --proto_path=./account --go_out=./account/pb ./account/account.proto`

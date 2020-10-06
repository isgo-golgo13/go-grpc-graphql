# go-grpc-graphql
Go (1.15.x) Google GRPC, GraphQL and Jaegar distributed tracing injection (including Dockerfile)


### Compiling the microservice {account, order, order_catalog}.proto files

For each of the services (account, order, order_catalog, graphql), `cd` into the `services/{account|order|order_catalog|graphql}`  directory and run:

`protoc --proto_path=./{account, order, order_catalog, graphql} --go_out=./{account, order, order_catalog, graphql}/pb ./{account, order, order_catalog, graphql}/{account, order, order_catalog, graphql}.proto`


For `services/account` issue the following (from directory services/account):

`protoc --proto_path=./account --go_out=./account/pb ./account/account.proto`


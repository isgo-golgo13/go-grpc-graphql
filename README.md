# go-grpc-graphql
Go (1.15.x) Google GRPC, GraphQL and Jaegar distributed tracing injection (including Dockerfile)


### Compiling the microservice {account, order, order_catalog}.proto files

For each of the services (account, order, order_catalog, graphql), `cd` into the `services/{account|order|order_catalog|graphql}`  directory and run:

`protoc --proto_path=./{account, order, order_catalog, graphql} --go_out=./{account, order, order_catalog, graphql}/pb ./{account, order, order_catalog, graphql}/{account, order, order_catalog, graphql}.proto`


##### For `services/account` issue the following (from directory services/account):

`protoc --proto_path=./account --go_out=./account/pb ./account/account.proto`


For `services/order` issue the following (from directory services/account):

`protoc --proto_path=./order --go_out=./order/pb ./order/ordert.proto`


For `services/order_catalog` issue the following (from directory services/account):

`protoc --proto_path=./order_catalog --go_out=./order_catalog/pb ./order_catalog/order_catalog.proto`


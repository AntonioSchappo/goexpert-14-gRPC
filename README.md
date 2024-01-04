# Goexpert-14-gRPC

This project is a simple implementation of a gRPC server using Go.
We are using [Evans](https://github.com/ktr0731/evans) in order to simulate the client side.
It is part of the Go Expert Course of [FullCycle Development](https://goexpert.fullcycle.com.br/pos-goexpert/).

## Commands to run

On the root of the project use the tidy command to organize the dependencies:

```sh
go mod tidy
```

Start the sqlite3 table using the following commands:

```sh
sqlite3 data.db
create table categories (id string, name string, description string);
```

Then run the main function using the command below:
```sh
go run cmd/server/server.go
```

With Evans installed, use the command below in order to test the server in REPL mode:
```sh
evans -r repl
```
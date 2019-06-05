# Coin & Purse Ledger Interface ![MoneyBag](./img/moneybag.png)

## Overview

Contains the grpc proto file and auto-generated client and server grpc code.

## Code generation instructions

These instruction require that the protoc:0.1.0 Docker image be built (or pulled if
in a registry) before running. Here is the
[repo](https://github.com/Drewan-Tech/protoc) to build the image.

### Go server code generation instructions
This command is run at the top level in this repo.
```Bash
docker run --rm --mount type=bind,source="$(pwd)"/src,target=/go/src/ledger_interface protoc:0.1.0 --proto_path=/go/src/ledger_interface/proto --go_out=/go/src/ledger_interface/go /go/src/ledger_interface/proto/ledger.proto
```

### JS client code generation instructions
```Bash
```

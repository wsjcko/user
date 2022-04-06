# User Service

This is the User service

Generated with

```
 docker run --rm -v  $PWD:$PWD -w $PWD micro/micro new user
```

## Usage

Generate the proto code
参考 Makefile 安装 protoc-gen-micro， protoc-gen-openapi

```
protoc --proto_path=. --micro_out=. --go_out=:. proto/pb/user.proto

make proto
```

Run the service

```
micro run .
```
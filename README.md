# shared

## Development Guide

### Generate Proto
```
cd portal (or any services)
protoc --proto_path=../shared/proto/api --go_out=internal/proto/out/api --go_opt=paths=source_relative --go-grpc_opt=paths=source_relative --go-grpc_out=internal/proto/out/api portal/user.proto mortalkin/user.proto mortalkin/game.proto
protoc --proto_path=../shared/proto/event --go_out=internal/proto/out/event --go_opt=paths=source_relative --go-grpc_opt=paths=source_relative --go-grpc_out=internal/proto/out/event event_user.proto
```

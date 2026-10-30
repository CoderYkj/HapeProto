# HapeProto

Shared protobuf contracts for HapeServer and HapeGateway.

- `proto/player/v1/player.proto` → `playerv1`: player TCP wire.
- `proto/world/v1/world.proto` → `worldv1`: world command/response and state delta.

Regenerate:

```bash
protoc --go_out=. --go_opt=module=github.com/CoderYkj/HapeProto \
  proto/world/v1/world.proto proto/player/v1/player.proto
```
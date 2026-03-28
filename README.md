# protos

Protobuf definitions and generated Go code for VoidRoute services.

## Structure

```
proto/                  # Source .proto files
  analytics/
    v1/
      analytics.proto
gen/                    # Generated code (do not edit manually)
  analytics/
    v1/
      analytics.pb.go
      v1connect/
        analytics.connect.go
buf.yaml
buf.gen.yaml
```

## Usage

```bash
go get github.com/voidroute/protos@latest
```

```go
import analyticsv1 "github.com/voidroute/protos/gen/analytics/v1"
```

## Generating code

Install [buf](https://buf.build/docs/installation):

```bash
brew install bufbuild/buf/buf # Mac OS / Linux
scoop install buf # Windows
```

Generate:

```bash
buf generate
```

## Versioning

Breaking changes are introduced under a new version directory (e.g. `v2/`). Non-breaking changes can be added to existing versions.
Drone plugin to upload build artifacts to S3. You are able to upload any kind of
build artifact onto S3 or any other s3-compatible storage system.

## Examples

```yaml
kind: pipeline
name: default

steps:
- name: step name
  image: dronehippie/s3:1
  settings: []
```

## Parameters

dummy
: dummy

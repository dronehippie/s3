# s3

[![Current Tag](https://img.shields.io/github/v/tag/dronehippie/s3?sort=semver)](https://github.com/dronehippie/s3) [![Build Status](http://drone.webhippie.de/api/badges/dronehippie/s3/status.svg)](http://drone.webhippie.de/api/badges/dronehippie/s3) [![Join the Matrix chat at https://matrix.to/#/#webhippie:matrix.org](https://img.shields.io/badge/matrix-%23webhippie-7bc9a4.svg)](https://matrix.to/#/#webhippie:matrix.org) [![Docker Size](https://img.shields.io/docker/image-size/dronehippie/s3/latest)](https://hub.docker.com/r/dronehippie/s3) [![Docker Pulls](https://img.shields.io/docker/pulls/dronehippie/s3)](https://hub.docker.com/r/dronehippie/s3) [![Go Reference](https://pkg.go.dev/badge/github.com/dronehippie/s3.svg)](https://pkg.go.dev/github.com/dronehippie/s3) [![Go Report Card](https://goreportcard.com/badge/github.com/dronehippie/s3)](https://goreportcard.com/report/github.com/dronehippie/s3) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/2ea9d9ee23af4c0f871c9dd46cbc71ab)](https://www.codacy.com/gh/dronehippie/s3/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=dronehippie/s3&amp;utm_campaign=Badge_Grade)

Drone plugin to upload build artifacts to S3. For the usage information and a listing of the available options please take a look at the [documentation](https://dronehippie.github.io/s3/).

## Build

Build the binary with the following command:

```console
export GOOS=linux
export GOARCH=amd64

make build
```

## Docker

Build the image with the following command:

```console
docker build \
  --label org.opencontainers.image.source=https://github.com/dronehippie/s3 \
  --label org.opencontainers.image.revision=$(git rev-parse --short HEAD) \
  --label org.opencontainers.image.created=$(date -u +"%Y-%m-%dT%H:%M:%SZ") \
  --file docker/Dockerfile.amd64 --tag dronehippie/s3 .
```

## Usage

```console
docker run --rm \
  -e PLUGIN_DUMMY="dummy" \
  -v $(pwd):$(pwd) \
  -w $(pwd) \
  dronehippie/s3
```

## Security

If you find a security issue please contact [thomas@webhippie.de](mailto:thomas@webhippie.de) first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

-   [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```console
Copyright (c) 2021 Thomas Boerger <thomas@webhippie.de>
```

# mod_process_security RPM Packaging

[![Build Status](https://github.com/jfut/mod_process_security-rpm/workflows/test/badge.svg?branch=master)](https://github.com/jfut/mod_process_security-rpm/actions?query=workflow%3Atest)

## Usage

```
Usage:
    build [-d] [-h] BUILD_IMAGE_NAME

    Options:
        -d Debug mode.

    Build for CentOS 7:
        build -i centos:7
```

## Build RPM Packages with Docker

You can build RPM packages in Docker.

```
./build
```

- Debug shell

```
./build -d
/pkg/build-rpm /pkg/rpmbuild mod_process_security.spec
```

## Release tag

e.g.:

```
git tag -a v1.1.4-1 -m "v1.1.4-1"
git push origin refs/tags/v1.1.4-1
```


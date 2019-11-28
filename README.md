# mod_process_security RPM Packaging

[![Build Status](https://github.com/jfut/mod_process_security-rpm/workflows/test/badge.svg?branch=master)](https://github.com/jfut/mod_process_security-rpm/actions?query=workflow%3Atest)

RPM Packaging for [mod_process_security](https://github.com/matsumotory/mod_process_security).

## Install an RPM package

- [Download](https://github.com/jfut/mod_process_security-rpm/releases)
- `yum install mod_process_security-x.y.z-n.elx.x86_64.rpm`
- Edit `/etc/httpd/conf.d/mod_process_security.conf`
- `systemctl restart httpd.service`

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

## License

MIT


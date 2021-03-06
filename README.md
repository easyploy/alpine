# Alpine Docker Container Image

[![Build Status](https://github.com/easyploy/alpine/workflows/Build%20docker%20image/badge.svg)](https://github.com/easyploy/alpine/actions)
[![Docker Pulls](https://img.shields.io/docker/pulls/easyploy/alpine.svg)](https://hub.docker.com/r/easyploy/alpine)
[![Docker Stars](https://img.shields.io/docker/stars/easyploy/alpine.svg)](https://hub.docker.com/r/easyploy/alpine)
[![Docker Layers](https://images.microbadger.com/badges/image/easyploy/alpine.svg)](https://microbadger.com/images/easyploy/alpine)

This is a basic alpine image used in Easyploy's docker images

## Docker Images

❗For better reliability we release images with stability tags (`easyploy/alpine:3-X.X.X`) which correspond to [git tags](https://github.com/easyploy/alpine/releases). We strongly recommend using images only with stability tags. 

About images:

* All images based on Alpine Linux
* Base image: [alpine](https://hub.docker.com/r/_/alpine)
- [GitHub actions builds](https://github.com/easyploy/alpine/actions) 
* [Docker Hub](https://hub.docker.com/r/easyploy/alpine) 

[_(Dockerfile)_]: https://github.com/easyploy/alpine/tree/master/Dockerfile

Supported tags and respective `Dockerfile` links:

* `3.13`, `3`, `latest` [_(Dockerfile)_]
* `3.12` [_(Dockerfile)_]
* `3.11` [_(Dockerfile)_]
* `3.10` [_(Dockerfile)_]
* `3.13-dev`, `3-dev`, `dev` [_(Dockerfile)_]

All images built for `linux/amd64` and `linux/arm64`

## Scripts

This image contains the following helper scripts:

* `compare_semver` - compares two semantic versions
* `exec_init_scripts` - execute all `.sh` scripts from `/docker-entrypoint-init.d/`. Useful to have in every docker image
* `gen_ssh_keys` - generates SSH keys
* `gen_ssl_certs` - generate SSL certificates
* `get_archive` - copies (or downloads) and unpacks an archive
* `gpg_verify` - verify GPG signature from a list of key servers
* `gpg_decrypt` - decrypt an artifact that contains GPG signature
* `wait_for` - executes a command with for N times with N timeout until it return 0

See [`test.sh`](https://github.com/easyploy/alpine/blob/master/test.sh) for examples.

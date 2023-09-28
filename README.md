# Terowongan

Terowongan (IPA: /təroˈwɔŋan/) means tunnel in indonesian language. Terowongan itself is an implementation of HTTP Tunneling in Rust.

## Motivation

While there's already a lot of HTTP tunneling implementation in general. Like [A LOT](https://github.com/anderspitman/awesome-tunneling). This project isn't really meant to compete with all of those existing project. But rather just an exercise in Rust on how to make a functional software that (maybe) could work in production.

## Usage

WIP

## Development Plan

- [ ] Implement HTTP Connect host
  - [ ] Connect worker function
  - [ ] Subdomain (with SNI) support for Connect
  - [ ] Authentication & Authorization
- [ ] Implement HTTP Connect client
  - [ ] Start a Connect tunnel with the host on a port
  - [ ] Multiple port Connection

## Docs

Go to [docs](./docs/README.md) to see deeper explanation on the software.

## Maintainer

fauh45

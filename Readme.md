
# name

  super lame quick hack of a delegation proxy that fixes
  a weird tarball assumption that npm makes about the host.

## Installation

```
$ npm install -g segmentio/npm-proxy
```

## Usage

```
  Usage: npm-proxy [options] <registry-url ...>

  Options:

    -h, --help         output usage information
    -p, --port <port>  port to listen on [3333]
    -u, --url <url>    registry url `ex: https://registry.segment.io`
```

## Example

```js
$ nohup npm-proxy \
  -p 3000 \
  -u https://user:pass@registry.segment.io \
  http://localhost:5984/registry/_design/app/_rewrite \
  http://registry.npmjs.org
```

# License

  MIT
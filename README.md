# Helix

[![Build Status](https://travis-ci.org/penberg/helix.svg?branch=master)](https://travis-ci.org/penberg/helix)

Helix is an ultra low-latency market data feed handler written in C++. It provides an API to trading applications that normalizes market data updates from multiple feeds.

Helix core does not include networking functionality and expects applications to provide raw packet data.

## Building

Helix requires libuv 1.0 or later. If you build it from sources, you need to tell pkg-config where to find the configuration files:

```
export PKG_CONFIG_PATH=/usr/local/lib/pkgconfig/
```

## Features

### Core

* [x] C++ API
* [x] C binding
* [x] Order book view
* [x] Data normalization
* [x] Data filtering
* [ ] Order book aggregation
* [ ] Synthetic NBBO
* [ ] Retransmission requests

### Protocols

* NASDAQ OMX Nordic
  * [x] Equity Total-View ITCH
  * [x] MoldUDP
  * [x] SoupFILE

## License

Copyright © 2015 Pekka Enberg

Helix is distributed under the 2-clause BSD license. See [LICENSE](https://github.com/penberg/helix/blob/master/LICENSE) for the full license text.

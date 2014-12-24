docker-hipache
==============

Docker container for [Hipache](https://github.com/hipache/hipache) based on
`node:0.11.14`, which is unstable but I needed this patch:
https://github.com/joyent/node/commit/bb909ad64285194b3d02322e3fb4b17ff5192c50
to use a more secure and reliable SSL/TLS layer.

**Important:** this version is patched to support a
[`force-https`](https://github.com/willdurand/docker-hipache/tree/force-https)
feature. By setting the `server.forceHttps` configuration option to `true`, all
traffic from `http` will be redirected to `https`.

# This fork
This fork compiles a minimal version of FFmpeg to include in a web browser (wasm).
The minimal build includes no codecs but supports all formats, allowing for probing and extracting streams with `copy`.

The main changes of this fork:
- `Dockerfile` disable all codecs, unnecessary builders and `esm` build.
- `ffmpeg-wasm.sh` remove link libraries

Building (using `make prd`, set to `-O3`) builds two binaries `packages/core/dist/umd/{ffmpeg-core.wasm,ffmpeg-core.wasm}`.
The `wasm` binary is roughly 3.8MB in size.

These binaries can be loaded using the `@ffmpeg/ffmpeg` package and served by the web server.

This project is looking for maintainers. If you are interested to give it a go, please email [me](mailto:jeromewus@gmail.com) to further discuss maintenance.

---
<p align="center">
  <a href="#">
    <img alt="ffmpeg.wasm" width="128px" height="128px" src="https://github.com/ffmpegwasm/ffmpeg.wasm/blob/main/apps/website/static/img/logo192.png"></img>
  </a>
</p>

# ffmpeg.wasm

ffmpeg.wasm is a pure Webassembly / Javascript port of FFmpeg. It enables video & audio record, convert and stream right inside browsers.

[![stability-experimental](https://img.shields.io/badge/stability-experimental-orange.svg)](https://github.com/emersion/stability-badges#experimental)
[![Node Version](https://img.shields.io/node/v/@ffmpeg/ffmpeg.svg)](https://img.shields.io/node/v/@ffmpeg/ffmpeg.svg)
[![Actions Status](https://github.com/ffmpegwasm/ffmpeg.wasm/workflows/CI/badge.svg)](https://github.com/ffmpegwasm/ffmpeg.wasm/actions)
![npm (tag)](https://img.shields.io/npm/v/@ffmpeg/ffmpeg/latest)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/ffmpegwasm/ffmpeg.wasm/graphs/commit-activity)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Downloads Total](https://img.shields.io/npm/dt/@ffmpeg/ffmpeg.svg)](https://www.npmjs.com/package/@ffmpeg/ffmpeg)
[![Downloads Month](https://img.shields.io/npm/dm/@ffmpeg/ffmpeg.svg)](https://www.npmjs.com/package/@ffmpeg/ffmpeg)
[![Netlify Status](https://api.netlify.com/api/v1/badges/1943b6d3-45ad-4b46-bfba-cb8d5716604c/deploy-status)](https://app.netlify.com/sites/ffmpegwasm/deploys)

Join us on Discord!

[![Discord](https://dcbadge.vercel.app/api/server/NjGMaqqfm5)](https://discord.gg/NjGMaqqfm5)

## Documentation

- [Introduction](https://ffmpegwasm.netlify.app/docs/overview)
- [Getting
    Started](https://ffmpegwasm.netlify.app/docs/getting-started/installation)
- [API](https://ffmpegwasm.netlify.app/docs/api/ffmpeg/)
- [FAQ](https://ffmpegwasm.netlify.app/docs/faq)
- [Contribution](https://ffmpegwasm.netlify.app/docs/contribution/core)

Please sponsor ffmpeg.wasm to make it sustainable. :heart:

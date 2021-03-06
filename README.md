# `twitchgg-api-worker`

[![CI](https://github.com/jebibot/twitchgg-worker/actions/workflows/main.yml/badge.svg?branch=main&event=push)](https://github.com/jebibot/twitchgg-worker/actions/workflows/main.yml)

The API Backend for twitchgg.tv services.

## ๐ Getting Started

This project is generated from `worker-typescript-template`. [Wrangler](https://developers.cloudflare.com/workers/cli-wrangler/install-update) 1.17 or newer is required. If you are not already familiar with the tool, we recommend that you install the tool and configure it to work with your [Cloudflare account](https://dash.cloudflare.com). Documentation can be found [here](https://developers.cloudflare.com/workers/tooling/wrangler/).

### ๐ฉ ๐ป Developing

[`src/index.ts`](./src/index.ts) calls the request handler in [`src/handler.ts`](./src/handler.ts), and will return the [request method](https://developer.mozilla.org/en-US/docs/Web/API/Request/method) for the given request.

### ๐งช Testing

This template comes with jest tests which simply test that the request handler can handle each request method. `npm test` will run your tests.

### โ๏ธ Formatting

This template uses [`prettier`](https://prettier.io/) to format the project. To invoke, run `npm run format`.

### ๐ Previewing and Publishing

For information on how to preview and publish your worker, please see the [Wrangler docs](https://developers.cloudflare.com/workers/tooling/wrangler/commands/#publish).

## ๐คข Issues

If the problem is with Wrangler, please file an issue [here](https://github.com/cloudflare/wrangler/issues).

## โ ๏ธ Caveats

The `service-worker-mock` used by the tests is not a perfect representation of the Cloudflare Workers runtime. It is a general approximation. We recommend that you test end to end with `wrangler dev` in addition to a [staging environment](https://developers.cloudflare.com/workers/tooling/wrangler/configuration/environments/) to test things before deploying.

# clone-api

If you're working with a client that doesn't use staging and the API you depend on keeps crashing, or working from a flaky internet connection or none at all, this tool is for you.

`clone-api` is an npm package built with typescript, that you specify a list of endpoints via a yaml file for for it, and it will cache them for you and put up an http server for you to use, so you won't be reliant on flaky APIs.

The yaml file scheme is simply an array of (AxiosRequestConfig)[https://github.com/axios/axios#request-config].

## how to use

- `yarn global add clone-api` / `npm i -g clone-api`.
- `clone-api start ./path/to/axios.description.of.my.api.yaml`

## What could work if we'd work on it

- suggestions?
- error handling
- support for custom responses via the yaml file
- support json in addition to yaml
- support same url with different methods (`/record` with GET, PUT, DELETE, etc)
- support for images
- maybe support background refresh of api
- far far future: plugin for webpack
- maybe auto generate typescript definitions for the endpoints in a nice way.

## Help me expand this package

Do you want functionality not yet coded in this package? send me an email and lets pair program on this.

## buzzwords for seo

This npm package takes an API offline to use. Mirror any API on localhost. Open source software for the commandline for APIs.

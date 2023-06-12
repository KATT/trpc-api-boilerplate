# tRPC API Boilerplate

[![CI][ci-badge]][ci-url]

Minimal [tRPC](https://trpc.io/) API boilerplate. Easily build &amp; publish fully typesafe APIs that any frontend can consume.

Monorepos are great, but sometimes we are targeting backend and frontend as separate (mono)repositories:

- separation/encapsulation of backend and frontend domain (except what must be exposed to both through API).
- separation of backend and frontend developers (larger teams/companies).
- separation of backend and frontend CI/CD pipelines.

... in that case checkout this boilerplate.

## Running

_Easily set up a local development environment_

- fork & clone repo
- `npm install`
- make changes to tRPC API & push
- consume tRPC API [package](https://www.npmjs.com/package/trpc-api-boilerplate) with any frontend app 🚀

## Example Repo

Example frontend app repository - [tRPC Frontend Boilerplate](https://github.com/mkosir/trpc-fe-boilerplate)

## Avoid publishing package?

If for whatever reason publishing a package is not an option:

- privacy concerns
- faster development iterations - skip CI (BE/FE monorepo look and feel)
- ...

Run `npm run trpc-api-export` and push code changes. In your [frontend app](https://github.com/mkosir/trpc-fe-boilerplate/blob/main/package.json#L6) run `npm run trpc-api-import`.

<!-- Badges -->

[ci-badge]: https://github.com/mkosir/trpc-api-boilerplate/actions/workflows/CI.yml/badge.svg
[ci-url]: https://github.com/mkosir/trpc-api-boilerplate/actions/workflows/CI.yml

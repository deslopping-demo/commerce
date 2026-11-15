# Commerce platform

A commerce backend: carts, orders, payments, customers and the admin
dashboard. It is built on [Medusa](https://github.com/medusajs/medusa).

> **This is a demonstration repository.** It exists to show
> [Deslopping](https://deslopping.app) at work on a real codebase. The code is
> Medusa v2.18.0, copied without its documentation site and its project files.
> Medusa is © Medusajs and licensed under the MIT License; see
> [LICENSE](LICENSE). Medusa's authors have nothing to do with this
> demonstration and do not endorse it.

## Layout

| Path | What lives there |
| --- | --- |
| `packages/modules/` | One module per domain: `payment`, `order`, `cart`, `auth`, `customer` and the rest |
| `packages/core/` | The framework, shared types, workflows and utilities the modules build on |
| `packages/medusa/` | The HTTP API: admin and store routes |
| `packages/admin/` | The admin dashboard |
| `integration-tests/` | Tests that run the API against a real database |

## Running it

```sh
yarn install
yarn build
yarn test
```

## Reviews

Changes to payments and sign-in are reviewed by the people named in
[CODEOWNERS](CODEOWNERS). Every pull request needs one approval.

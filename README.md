# @zondax/ledger-peaq-js

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![npm version](https://badge.fury.io/js/%40zondax%2Fledger-peaq.svg)](https://badge.fury.io/js/%40zondax%2Fledger-peaq)
[![GithubActions](https://github.com/zondax/ledger-peaq-js/actions/workflows/main.yml/badge.svg)](https://github.com/Zondax/ledger-peaq-js/blob/main/.github/workflows/main.yaml)
[![CodeFactor](https://www.codefactor.io/repository/github/zondax/ledger-peaq-js/badge)](https://www.codefactor.io/repository/github/zondax/ledger-peaq-js)

![zondax_light](docs/zondax_light.png#gh-light-mode-only)
![zondax_dark](docs/zondax_dark.png#gh-dark-mode-only)

This package provides a basic client library to communicate with a Peaq App running in a Ledger Nano S/S+/X devices

We recommend using the npmjs package in order to receive updates/fixes.

Use `yarn install` to avoid issues.

# Available commands

| Operation          | Response                    | Command                     |
| ------------------ | --------------------------- | --------------------------- |
| getVersion         | app version                 | ---------------             |
| appInfo            | name, version, flags, etc   | ---------------             |
| deviceInfo         | fw and mcu version, id, etc | Only available in dashboard |
| signRawBytes       | signed message              | path + message              |
| signETHTransaction | signed message              | path + message              |
| getETHAddress      | pubkey + address            | path                        |

# Testing with real devices

It is possible to test this package with a real Ledger Nano device. To accomplish that, you will need to follow these steps:

- Install the application in the Ledger device
- Install the dependencies from this project
- Run tests

```shell script
yarn install
yarn test:integration
```

# Who we are?

We are Zondax, a company pioneering blockchain services. If you want to know more about us, please visit us at [zondax.ch](https://zondax.ch)

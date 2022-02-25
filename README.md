# boomerang  • [![tests](https://github.com/abigger87/boomerang/actions/workflows/tests.yml/badge.svg)](https://github.com/abigger87/boomerang/actions/workflows/tests.yml) [![lints](https://github.com/abigger87/boomerang/actions/workflows/lints.yml/badge.svg)](https://github.com/abigger87/boomerang/actions/workflows/lints.yml) ![GitHub](https://img.shields.io/github/license/abigger87/boomerang) ![GitHub package.json version](https://img.shields.io/github/package-json/v/abigger87/boomerang)

An Owned, Gas Efficient ERC721 For Testing In Prod (Mainnet).

## Overview

A gas efficient ERC721 contract that allows the `OWNER` to recover gas costs.

Deployed to Mainnet at [`0x9172c52bf412de76e080bd595f8f8c55f0ff867c`](https://etherscan.io/address/0x9172c52bf412de76e080bd595f8f8c55f0ff867c).

Deployed to Rinkeby at [`0x715da5e53526bedac9bd96e8fdb7efb185d1b6ca`](https://rinkeby.etherscan.io/address/0x715da5e53526bedac9bd96e8fdb7efb185d1b6ca).

Deployer: [`0xc9ab63915c6738c8ce5ca245979203bfa3f2499f`](https://etherscan.io/address/0xc9ab63915c6738c8ce5ca245979203bfa3f2499f).

#### Known Errors

Hardhat issue:
```sh
Error HH12: Trying to use a non-local installation of Hardhat, which is not supported.
Please install Hardhat locally using npm or Yarn, and try again.
```

> Make sure hardhat is installed by running `yarn` or manually adding hardhat to dev dependencies using `yarn add --dev hardhat`.




## Blueprint

```ml
lib
├─ ds-test — https://github.com/dapphub/ds-test
├─ forge-std — https://github.com/brockelmore/forge-std
├─ solmate — https://github.com/Rari-Capital/solmate
├─ clones-with-immutable-args — https://github.com/wighawag/clones-with-immutable-args
src
├─ tests
│  └─ \( ._. )/
└─ Boomerang — "The Gas Optimized ERC721 Contract"
```

## Development

#### First time with Forge/Foundry?

See the official Foundry installation [instructions](https://github.com/gakonst/foundry/blob/master/README.md#installation).

Don't have [rust](https://www.rust-lang.org/tools/install) installed?
Run
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

Then, install the [foundry](https://github.com/gakonst/foundry) toolchain installer (`foundryup`) with:
```bash
curl -L https://foundry.paradigm.xyz | bash
```

Now that you've installed the `foundryup` binary,
anytime you need to get the latest `forge` or `cast` binaries,
you can run `foundryup`.

So, simply execute:
```bash
foundryup
```

🎉 Foundry is installed! 🎉

#### Configure Foundry

Using [foundry.toml](./foundry.toml), Foundry is easily configurable.

#### Install DappTools

Install DappTools using their [installation guide](https://github.com/dapphub/dapptools#installation).

#### Setup

```bash
make
# OR #
make setup
```

#### Build

```bash
make build
```

#### Run Tests

```bash
make test
```

## License

[AGPL-3.0-only](https://github.com/abigger87/boomerang/blob/master/LICENSE)

# Acknowledgements

- [foundry-starter](https://github.com/abigger87/foundry-starter)
- [foundry](https://github.com/gakonst/foundry)
- [solmate](https://github.com/Rari-Capital/solmate)
- [forge-std](https://github.com/brockelmore/forge-std)
- [clones-with-immutable-args](https://github.com/wighawag/clones-with-immutable-args).
- [foundry-toolchain](https://github.com/onbjerg/foundry-toolchain) by [onbjerg](https://github.com/onbjerg).
- [forge-template](https://github.com/FrankieIsLost/forge-template) by [FrankieIsLost](https://github.com/FrankieIsLost).
- [Georgios Konstantopoulos](https://github.com/gakonst) for [forge-template](https://github.com/gakonst/forge-template) resource.

## Disclaimer

_These smart contracts are being provided as is. No guarantee, representation or warranty is being made, express or implied, as to the safety or correctness of the user interface or the smart contracts. They have not been audited and as such there can be no assurance they will work as intended, and users may experience delays, failures, errors, omissions, loss of transmitted information or loss of funds. The creators are not liable for any of the foregoing. Users should proceed with caution and use at their own risk._

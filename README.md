# Forbitswap Interface

[![Lint](https://github.com/Forbitswap/forbitswap-interface/workflows/Lint/badge.svg)](https://github.com/Forbitswap/forbitswap-interface/actions?query=workflow%3ALint)
[![Tests](https://github.com/Forbitswap/forbitswap-interface/workflows/Tests/badge.svg)](https://github.com/Forbitswap/forbitswap-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for Forbitswap -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [forbitswap.com](https://forbitswap.com/)
- Interface: [app.forbitswap.com](https://app.forbitswap.com)
- Docs: [forbitswap.com/docs/](https://forbitswap.com/docs/)
- Twitter: [@ForbitswapProtocol](https://twitter.com/ForbitswapProtocol)
- Reddit: [/r/Forbitswap](https://www.reddit.com/r/Forbitswap/)
- Email: [contact@forbitswap.com](mailto:contact@forbitswap.com)
- Discord: [Forbitswap](https://discord.gg/Y7TF6QA)
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Accessing the Forbitswap Interface

To access the Forbitswap Interface, use an IPFS gateway link from the
[latest release](https://github.com/Forbitswap/forbitswap-interface/releases/latest), 
or visit [app.forbitswap.com](https://app.forbitswap.com).

## Listing a token

Please see the
[@forbitswap/default-token-list](https://github.com/forbitswap/default-token-list) 
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"` 

Note that the interface only works on testnets where both 
[Forbitswap](https://forbitswap.com/docs/smart-contracts/factory/) and 
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.** 
CI checks will run against all PRs.

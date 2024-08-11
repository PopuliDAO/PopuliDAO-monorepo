# PopuliDAO-monorepo
A DAO platform with proof of personhood and a token cap per individual implemented to maintain decentralization and limit disproportionate influence by whales.

## Repository Structure
We have two submodules :
- The `PopuliDAO-SC` repository is the smart contract repository.
- The `PopuliDAO-UI` repository is the frontend repository.

# `PopuliDAO-SC` Repo

## Usage

### Installation

```shell
cp .env.example .env
npm install
npx hardhat compile
npx hardhat test
```

## Developer Protal

https://developer.worldcoin.org/login

### Deployments

| Network          | Address                                    | Abi - Etherscan                                                                                                                                                                                 |
| ---------------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| optimism_sepolia | 0x4d12143B1fE21e353eB95b528D051e51c07Aee23 | MyToken <a href="./abis/MyToken.json">abi</a> - <a href="https://sepolia-optimism.etherscan.io/address/0x4d12143B1fE21e353eB95b528D051e51c07Aee23#code">etherscan</a>                           |
| optimism_sepolia | 0x7B5e2b49a63e1c9780E70241061Bcb5223f2C831 | MyGovernorDao <a href="./abis/MyGovernorDao.json">abi</a> - <a href="https://sepolia-optimism.etherscan.io/address/0x7B5e2b49a63e1c9780E70241061Bcb5223f2C831#code">etherscan</a>               |
| optimism_sepolia | 0x170180963693BFAC5E9265045f5862557E4d71f4 | WorldIdMock <a href="./abis/WorldIdMock.json">abi</a> - <a href="https://sepolia-optimism.etherscan.io/address/0x170180963693BFAC5E9265045f5862557E4d71f4#code">etherscan</a>                   |
| optimism_sepolia | 0x8f312ABa012fEe5948dbc7d7F7612462c9Ba95d2 | WorldVerify <a href="./abis/WorldVerify.json">abi</a> - <a href="https://sepolia-optimism.etherscan.io/address/0x8f312ABa012fEe5948dbc7d7F7612462c9Ba95d2#code">etherscan</a>                   |
| optimism_sepolia | 0x85C5b0bDeBaB547C0D11e5bD7bFECE49DCcc874d | MyGovernorDaoFactory <a href="./abis/MyGovernorDaoFactory.json">abi</a> - <a href="https://sepolia-optimism.etherscan.io/address/0x85C5b0bDeBaB547C0D11e5bD7bFECE49DCcc874d#code">etherscan</a> |

#### Commands

Mock deployment:
`npx hardhat run scripts/MockDeployments.ts [--network <your_network>]`

Integrated deployment:
`npx hardhat run scripts/deployments.js --network <your-network>`

## Integrations

Source: https://docs.worldcoin.org/reference/address-book

### Optimism Mainnet

```
World ID Router:   optimism.id.worldcoin.eth
Bridged World ID:  0xB3E7771a6e2d7DD8C0666042B7a07C39b938eb7d
```

### Optimism Sepolia Testnet

```
World ID Router:   0x11cA3127182f7583EfC416a8771BD4d11Fae4334
Bridged World ID:  0xf07d3efadD82A1F0b4C5Cc3476806d9a170147B
```

### Ethereum Mainnet

```
World ID Router:   id.worldcoin.eth
Identity Manager:  0xf7134CE138832c1456F2a91D64621eE90c2bddEa
```

### Ethereum Sepolia Testnet

```
World ID Router:   0x469449f251692e0779667583026b5a1e99512157
Identity Manager:  0xb2ead588f14e69266d1b87936b75325181377076
```

## Deployments

### Latest Optimism Sepolia deployments




# `PopuliDAO-UI` Repo

This is built using
- NextJS
- TypeScript
- Wagmi
- viem
- IDKit
- TailwindCSS
- ShadCn
- Aceternity UI
  
## Getting Started

First install the dependencies:

```bash
pnpm i
#or
yarn
#or
npm i
```

Paste the project ids in the `.env`

Then, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Then, open `localhost:3000`



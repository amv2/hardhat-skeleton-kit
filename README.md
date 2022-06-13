# The HardHat Skeleton Kit
This kit was created to quickly build and verify hardhat projects without having to copy paste boiler plate code

# Install the dependencies
First install the necessary dependencies with:
```
yarn add --dev @chainlink/contracts @openzeppelin/contracts @nomiclabs/hardhat-ethers @nomiclabs/hardhat-etherscan @nomiclabs/hardhat-waffle chai dotenv ethereum-waffle ethers hardhat hardhat-deploy hardhat-gas-reporter solidity-coverage
```

Optional: If required, linters can be installed with:
```
yarn add --dev eslint solhint prettier prettier-plugin-solidity
```

```
{
  "name": "hardhat-skeleton-kit",
  "author": "amv2",
  "version": "1.0.0",
  "devDependencies": {
  },
  "scripts": {
    "test": "yarn hardhat test",
    "test:staging": "yarn hardhat test --network rinkeby",
    "lint": "yarn solhint 'contracts/*.sol'",
    "lint:fix": "yarn solhint 'contracts/*.sol' --fix",
    "format": "yarn prettier --write .",
    "coverage": "yarn hardhat coverage"
  }
}

```
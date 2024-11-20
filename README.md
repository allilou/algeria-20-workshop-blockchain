# algeria-20-workshop-blockchain
Workshop on blockchain for Algeria 2.0  2024 Edition

## Prerequisit 

- Docker
- Ad DevContainer extension to VSCode 

## Initialization

Install hardhat
```bash
npm install --save-dev hardhat
npx hardhat
```

Create the sample project
```bash
mkdir src
npx hardhat init
```
You'll be prompted to choose :
✔ What do you want to do? · Create a TypeScript project
✔ Hardhat project root: · /workspaces/algeria-20-workshop-blockchain/src
✔ Do you want to add a .gitignore? (Y/n) · y
✔ Help us improve Hardhat with anonymous crash reports & basic usage data? (Y/n) · n
✔ Do you want to install this sample project's dependencies with npm (@nomicfoundation/hardhat-toolbox)? (Y/n) · y


## Developement 

Open a terminal in VSCode 

Check `hardhat`
```bash
cd src
npx hardhat
npx hardhat compile
```

You can run your tests with
```bash
npx hardhat test
```

## Deploying contracts 

Start an etherum node for testing 
```bash
npx hardhat node
```

You Deploy the contrat for testing
```bash
npx hardhat ignition deploy ./ignition/modules/Lock.ts --network localhost
```

## Deploy the contrat using Web3JS

Install web3js
```bash
npm install --save-dev @nomicfoundation/hardhat-web3-v4 'web3@4'
```

Install web3js
```bash
npx hardhat run scripts/deploy.ts
```

## Accessing the contract from a Web3JS dApp

Check the React App
```bash
cd web
npm install
npm start
```

# Useful links 

- [https://hardhat.org/hardhat-runner/docs/getting-started](https://hardhat.org/hardhat-runner/docs/getting-started)
- [https://docs.web3js.org/guides/hardhat_tutorial/](https://docs.web3js.org/guides/hardhat_tutorial/)
- [https://medium.com/coinmonks/build-a-web-3-application-with-solidity-hardhat-react-and-web3js-61b7ff137885](https://medium.com/coinmonks/build-a-web-3-application-with-solidity-hardhat-react-and-web3js-61b7ff137885)
- [https://consensys.io/blog/consensys-announces-the-sunset-of-truffle-and-ganache-and-new-hardhat](https://consensys.io/blog/consensys-announces-the-sunset-of-truffle-and-ganache-and-new-hardhat)

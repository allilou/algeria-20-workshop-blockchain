# algeria-20-workshop-blockchain
Workshop on blockchain for Algeria 2.0  2024 Edition

## Prerequisit 

- Docker
- Ad DevContainer extension to VSCode 

## Initialization

Install hardhat
```bash
npm install --save-dev hardhat
npmx hardhat
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


# Useful links 

- [https://hardhat.org/hardhat-runner/docs/getting-started](https://hardhat.org/hardhat-runner/docs/getting-started)

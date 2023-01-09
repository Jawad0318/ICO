# Initial Coin Offering 
To build the smart contract we will be using Hardhat.
Hardhat is an Ethereum development environment and framework designed for full stack development in Solidity. 
In simple words you can write your smart contracts, deploy them, run tests, and debug your code.
To setup a Hardhat project, open up a terminal and execute these commands:
```
mkdir ICO
cd ICO
mkdir hardhat-tutorial
cd hardhat-tutorial
npm init --yes
npm install --save-dev hardhat
```
In the same directory where you installed Hardhat run:
```
npx hardhat
```
Make sure you select Create a Javascript Project and then follow the steps in the terminal to complete your Hardhat setup.

In the same terminal, install @openzeppelin/contracts as we will be importing Openzeppelin's ERC20 Contract and Openzeppelin's Ownable
 Contract in our CryptoDevToken contract.
 ```
 npm install @openzeppelin/contracts
 ```
We need to call the CryptoDevs Contract that you deployed for the previous level to check for owners of CryptoDev NFT's.
As we only need to call tokenOfOwnerByIndex and balanceOf methods, we can create an interface for CryptoDevs contract with only these two functions.
This way we save gas as we do not need to inherit and deploy the entire CryptoDevs Contract, but only a part of it.
check the repositry for detail knowledge about code
![ico](https://user-images.githubusercontent.com/98699119/211279831-a5450cbf-35bc-4c4b-beab-9ec0aaeefe0f.png)

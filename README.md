# avax-demo
- 文档：https://docs.avax.network/build/tutorials/smart-contracts/deploy-a-smart-contract-on-avalanche-using-remix-and-metamask/
- 测试网： https://testnet.snowtrace.io/
- 主网： https://snowtrace.io/
# Etherscan verification

To try out Etherscan verification, you first need to deploy a contract to an Ethereum network that's supported by Etherscan, such as Ropsten.

In this project, copy the .env.example file to a file named .env, and then edit it to fill in the details. Enter your Etherscan API key, your Ropsten node URL (eg from Alchemy), and the private key of the account which will send the deployment transaction. With a valid .env file in place, first deploy your contract:

```shell
npx hardhat run ./scripts/deploy.js --network avaxtest
``` 

Then, copy the deployment address and paste it in to replace `DEPLOYED_CONTRACT_ADDRESS` in this command:

```shell
npx hardhat verify --network avaxtest DEPLOYED_CONTRACT_ADDRESS "Hello, Hardhat!"
```


## graph
https://docs.avax.network/build/tutorials/tutorials-contest/pangolin-token-subgraph/

## chainlink
https://docs.avax.network/build/tutorials/tutorials-contest/red-dev-avalanche-chainlink-tutorial/


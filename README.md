
## software version
 
Ensure your `node` and `truffle` version is higher than these:
```sh
$ node -v
v14.17.6
$ truffle version
Truffle v5.3.7 (core: 5.3.7)
Solidity - >=0.6.6 <0.8.0 (solc-js)
Node v14.17.6
Web3.js v1.3.6
```
   
## environment variables
 
```
TEST_AMOUNT=0.05
BNB_AMOUNT=100
WALLET_ADDRESS=0x<your wallet address>
PRIVATE_KEY=<private key>
BSS_WSS=wss://bsc-ws-node.nariox.org:443
BSS_HTTPS=https://bsc-dataseed.binance.org/
MORALIS_BSC=https://speedy-nodes-nyc.moralis.io/<your account>/bsc/mainnet
```
 
## setup steps
  
1. Rename `.env.template` to `.env` and fill out required information
2. Configure `truffle-config.js` with appropriate parameters (if you deploy a contract)
3. Install node.js packages and compile a smart contract code
```sh
npm install
truffle compile
```
4. Migrate the contract to the network (confirm if you do this in BSC mainnet)
```sh
truffle migrate --network mainnet
```
 
## License
 
This library is licensed under the MIT License. 

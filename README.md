# ChainREST
## RUN
npm install

DEBUG=signapi:* npm start

## Functionality and connection to the blockchain

We use a third party module called `` fabric-network-simple: 1.1.0 `` which uses the official library of hyperledger fabric for JS to connect to a blockchain.

We need to specify the blockchain topology and configuration [line 6-routes/chain.js](https://github.com/agustin-marin/ChainREST/blob/main/routes/chain.js#L6)

We can use queryChaincode(readonly smartcontract operation) and invokeChaincode(read-write smartcontract operation) specifying method and parameters: [queryChaincode])(https://github.com/agustin-marin/ChainREST/blob/main/routes/chain.js#L98) and [invokeChaincode](https://github.com/agustin-marin/ChainREST/blob/main/routes/chain.js#L220), in order to execute smartcontracts on the blockchain.




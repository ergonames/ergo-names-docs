# Smart Contracts

Our smart contracts are built to ensure that minting funds are always secure for users. Written in ErgoScript, the smart contract is deployed on-chain. The contract has three possible outputs.

1. Mint an NFT
2. Issue a refund
3. Collect a royalty

If the contract mints an NFT, the funds the user deposited will be sent to the ErgoNames treasury. In return, the user receives a new ErgoNames NFT, ready to be used for receiving payments.

When issuing a refund, the user will receive all the funds back, minus a network fee to cover the cost of the on-chain transaction.

The royalty, which is set at 2%, only happens when a user sells the NFT on an auction house that supports royalties. This royalty uses the EIP-0024 standard.

A link to our smart contract can be found [here](https://github.com/ergonames/ergo-names-backend/blob/master/src/main/scala/contracts/ErgoNamesMintingContract.scala).
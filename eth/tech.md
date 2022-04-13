---
layout: default
---

# Ethereum

## Technical details

### Ethereum account

Ethereum has two types of account: 1) externally-owned account (EOA) 2) contract account. An EOA account is the account an Etherueum user uses to transact on the blockchain. An EOA account is made up of a pair of keys: public and private. The public key can be thought of as the account's address, while the private key can be thought of as an authentication key. In order to send ETH to another user, we initiate a transaction with the other user's address as the destination. We sign the transaction using our private key in order to authenticate it.

A private key consists of 64 hexadecimal characters (i.e. 256 bits/32 bytes). A user can generate a private key by 1) choosing a specific number, 2) randomly or 3) from a seed phrase (of words). The public key (128 hexadecimal characters/512 bits) is generated from the private key using the Elliptic Curve Digital Signature Algorithm. The address of an account is obtained by taking the last 40 hexadecimal characters (i.e. 160 bits/20 bytes) of the Keccak-256 hash of the public key and adding 0x to the beginning. Even though a private key is used to generate the public key, a public key *cannot* be used to generate a private key. A seed recovery phrase (e.g. Metamask) can be used to generate multiple public and private key pairs. As the Metamask wallet is deterministic, its seed phrase can be used to re-create the same key pairs in the same order.

#### References
- [Reddit post](https://www.reddit.com/r/CryptoCurrency/comments/papum2/creation_of_seed_phrase_private_key_and_public_key/)

### Ethereum transaction

For each Ethereum transaction to be successfuly included in the block, the user has to pay a gas fee to the miners. The total cost of gas depends on the number of units of gas (which depends on the computational complexity of the transaction) and the gas price. The gas price is denominated in gwei, with 1 gwei being equal to one billonth of 1 $ETH. The gas price consists of a base fee which is determined automatically from previous blocks, plus an additional priority fee (tip) that users can include to incentivize miners to include their transaction first before others. The user is also able to set a gas limit to limit the quantity of gas used. The total transaction fee is calculated by multiplying the units of gas by the gas price.

### Mempool
The mempool is a set of broadcasted transactions that have not been added into the blockchain. Miners decide which transactions to validate and include in the block, and often select transactions with higher fees.

### Contract ABI

A contract application binary interface (ABI) is similar to the term API (application programming interface). To interact with smart contracts that are stored on the blockchain, we typically need to call smart contract methods (i.e. functions) with certain parameters. When deploying a smart contract, the smart contract is compiled to EVM bytecode and stored on the blockchain associated with an address. To the EVM, the smart contract is just a sequence of bytecode. Method names and parameters have to be converted to byte representations to interact with the EVM, and similarly return values are encoded in bytes and need to be converted back to human readable formats.

#### References
- <https://www.quicknode.com/guides/solidity/what-is-an-abi>
- <https://ethereum.org/en/developers/docs/smart-contracts/compiling/>

### ERC20

The ERC-20 token standard is a standard interface that implements an API for fungible tokens. The interface requires various methods and events to be implemented. Examples include the `approve` and `transfer` methods. Any smart contract that implements the methods and events specified by the ERC-20 standard can be considered an ERC-20 token contract. Example implementations of ERC-20 token contracts have been written by OpenZeppelin and ConsenSys.

#### References
- <https://ethereum.org/en/developers/docs/standards/tokens/erc-20/>
- <https://eips.ethereum.org/EIPS/eip-20>

### ERC721
### GraphQL
### Cryptozombies tutorial

## On-chain arbitrage
- Trigger when arbitrage opportunity arises
- On-chain trade execution
    1. Deploy smart contract
    2. 0x API

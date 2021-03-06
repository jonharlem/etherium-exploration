###What is Ethereum?

Etherium is an open source platform to build and distribute decentralized applications of **Dapps**. By their very nature, decentralized applications have no middlemen or censors. Users interact within the systems -- social, financial, gaming, etc. -- all within a peer-to-peer fashion. The outcomes and ramifications of these interactions are only beginning to be explored: resistance to fraud or tampering, identity and verification solutions, voting, legal documents, reputation systems, social networks, etc. It is important to keep in mind that it took a number of years before social networks were developed for the web. The reality is that the biggest impacts will take time to be developed. 

Etherium borrows the concept of distributed consensus and cryptographic proof that makes Bitcoin so effective. The foundational building block in Etherium is a contract or program that lives on the distributed Ethereum network and follows a series of defined steps when it receives a transaction. Contracts can store data, send and receive transactions, and interact with other contracts holding data. The contacts themselves are maintained by the network, without any central ownership or control. The contracts are 'powered' by **Ether**. By its very design, Ethereum, is resistant to tampering or fraud.

###Accounts
(working on it...)

###Transactions
(working on it...)

###Gas
(working on it...)

###Storage
(working on it...)

###Developing on Ethereum

The Ethereum team has put in a lot of time and thought to make it possible for any developer to write and distribute decentralized applications.

###Smart Contracts

**Smart contracts** are account holding objects on the ethereum blockchain. They can contain functions, interact with other contracts, make decisions, store data, and send ether to others. Ethereum contracts are defined by their creators, but the execution of their services are controlled by the network itself. As long as the network exists, the contracts will be executable unless programmed to self destruct.

**But what can I do with smart contracts?**

The possibilities are extremely broad and only beginning to be explored. 

###Solidity Programming Language

[Solidity](https://github.com/ethereum/wiki/wiki/The-Solidity-Programming-Language) is an object-oriented language designed specifically for writing contracts in Ethereum. To be more specific, Solidity is often referred to as the first *contract-oriented* programming language. It is designed to help express agreements that encode ideas and relationships: ownership, identity, protections, etc.

**Example Storage:**
```solidity
contract SimpleStorage {
    uint storedData;
    function set(uint x) {
        storedData = x;
    }
    function get() constant returns (uint retVal) {
        return storedData;
    }
}
```

`uint storedData` declares a state variable called storedData of an uint or unsigned integer of 256 bits. It is easy to think of this as a single slot in a database that can be queried and altered by calling functions of the code owning the contract. In this case the functions 'set' and 'get' can be used to modify or retrieve the value of the variable.

You do not need the prefix `this.` as in Javascript.

####Vocab for Contracts
- Contract:
	
	> Collection of code (its functions)
- State:
	
	> A contract's data that resides at a specific address on the Ethereum blockchain

###Resources & Threads
---
**Videos**

- [Ethereum: the World Computer (1:28)](https://www.youtube.com/watch?v=j23HnORQXvs)

**How-To**

- [Hello World for Etherum](https://www.ethereum.org/greeter)

**Forums**

- [ethereum.org Forum](https://forum.ethereum.org/)
  - [etherium.org Mining Forum](https://forum.ethereum.org/categories/mining)
- [r/ethereum](https://www.reddit.com/r/ethereum)
- [r/EtherMining](https://www.reddit.com/r/EtherMining/)
- [Ethereum Stackexchange](http://ethereum.stackexchange.com/)

###What is missing from Ethereum?

While ethereum is 'Turing-complete', there are still a few things that you can't do with ethereum contracts.

> You can't look at the other transactions that occur in the block that you are currently executing in.  There is no off code that lets you load in the current block hash. You can't see the other transactions in the block. You can see other transaction in previous blocks, but only because of that hack. Because in ethereum you can access the hash of the previous block.	

- Transactional privacy. Think online auctions. 

##Blockchain

Information about blockchain technology in general.

###What is a blockchain?
Besides being a trending word/technology for 2016, a blockchain is a globally shared, transactional database. This means that everyone can read entries into the database by participating in the network. If you want to change something in the database you have to create a transaction which has to be accepted by all other nodes on the network. While your transaction is being applied to the network, no other transaction can alter it. 

The most famous blockchain is BitCoin. BitCoin is a ledger that lists the balances of all accounts in the electronic currency. If there is a transfer from one account to another, the transactional nature of the database will ensure that the amount is subtracted from one account and added to another account. If the transaction is not possible, the source account will not be modified. Every transaction is **cryptographically signed** by the sender/creator. This makes it incredibly hard to modify the database. In terms of BitCoin, this means that only the person holding a key to an account is allowed to modify that account.

###Merkle Tree

Merkle trees are a fundamental part of distributed systems like bockchains. They are used to detect differences between two large datasets by using minimal network transfers. While it is possible to make blockchains without Merkle trees, doing so poses scalability problems. 

Generally defined, Merkle trees or hash trees, are a way of hashing a large number of chunks into smaller chunks until the total number of hashes remaining becomes only one: the root hash.

###Proof-of-work

A **proof-of-work** is a piece of data which is difficult to produce, satisfies certain requirements, but is easy to verify by others. A proof-of-work is meant to be costly or time-consuming. Generally they are a random process with low probability that requires a great deal of trial and error before a valid proof is demonstrated.

Bitcoin uses the [Hashcash](https://en.wikipedia.org/wiki/Hashcash) as its proof-of-work system for its mining algorithm. Hashcash was originally used by several anti-spam systems.

Ethereum uses a proof-of-work called [Ethash](https://github.com/ethereum/wiki/wiki/Ethash).
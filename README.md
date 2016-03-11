###What is Ethereum?

Etherium is an open source platform to build and distribute decentralized applications of **Dapps**. By their very nature, decentralized applications have no middlemen or censors. Users interact within the systems -- social, financial, gaming, etc. -- all within a peer-to-peer fashion. The outcomes and ramifications of these interactions are only beginning to be explored: resistance to fraud or tampering, identity and verification solutions, voting, legal documents, reputation systems, social networks, etc. It is important to keep in mind that it took a number of years before social networks were developed for the web. The reality is that the biggest impacts will take time to be developed. 

Etherium borrows the concept of distributed consensus and cryptographic proof that makes Bitcoin so effective. The foundational building block in Etherium is a contract or program that lives on the distributed Ethereum network and follows a series of defined steps when it receives a transaction. Contracts can store data, send and receive transactions, and interact with other contracts holding data. The contacts themselves are maintained by the network, without any central ownership or control. The contracts are 'powered' by **Ether**. By its very design, Ethereum, is resistant to tampering or fraud.

###Developing on Ethereum

The Ethereum team has put in a lot of time and thought to make it possible for any developer to write and distribute decentralized applications.

###Smart Contracts

**Smart contracts** are account holding objects on the ethereum blockchain. They can contain functions, interact with other contracts, make decisions, store data, and send ether to others. Ethereum contracts are defined by their creators, but the execution of their services are controlled by the network itself. As long as the network exists, the contracts will be executable unless programmed to self destruct.

**But what can I do with smart contracts?**

The possibilities are extremely broad and only beginning to be explored. 

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

###Merkle Tree

Merkle trees are a fundamental part of distributed systems like bockchains. They are used to detect differences between two large datasets by using minimal network transfers. While it is possible to make blockchains without Merkle trees, doing so poses scalability problems. 

Generally defined, Merkle trees or hash trees, are a way of hashing a large number of chunks into smaller chunks until the total number of hashes remaining becomes only one: the root hash.

###Proof-of-work

A **proof-of-work** is a piece of data which is difficult to produce, satisfies certain requirements, but is easy to verify by others. A proof-of-work is meant to be costly or time-consuming. Generally they are a random process with low probability that requires a great deal of trial and error before a valid proof is demonstrated.

Bitcoin uses the [Hashcash](https://en.wikipedia.org/wiki/Hashcash) as its proof-of-work system for its mining algorithm. Hashcash was originally used by several anti-spam systems.

Ethereum uses a proof-of-work called [Ethash](https://github.com/ethereum/wiki/wiki/Ethash).
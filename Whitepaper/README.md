
![GitHub Logo](/Images/transparent_logo.png)

<br><br>
<center>
  <h1>Welcome to Earthchain</h1>
</center>
<br><br>

[Whitepaper Version 1.0 -alpha]<br><br>

This is the whitepaper for Earthchain Blockchain, a resource of the Herophilos community.
Earthchain represents the first step to industrialize blockchain technology, and by creating a lightweight blockchain we know that it will be compatible on all of the devices. 

This is the main source code repository for the Earthchain project. 

## Notes
    * Earthchain is still under active development and it is still evolving. 
    * We will be launching a live testnet of the Earthchain protocol in the near future. - [sign up here to join the testnet]  

<center>
  <h2>Abstract</h2>
</center>

Bitcoin and other distributed payment systems (also called cryptocurrencies or
simply blockchains) aim to provide a decentralized system for making and verifying payments. However, for traditional cryptocurrencies, including Bitcoin,
decentralization comes at the cost of scalability as each node needs to process
the entire system history upon joining the network. Asymptotically, verifying
a blockchain containing 푡 transactions requires 훺(푡) time (usually more than
linear in 푡 as bookkeeping is required to resolve transaction references during
verification). At the time of this writing, Bitcoin’s blockchain is over 250 GB
and contains over 500 M transactions (see Figure 1). Downloading and verifying
this history takes days on a typical laptop.
These resource requirements deter most users from running a full node that
stores and verifies the blockchain. As seen in Figure 2, the number of full nodes
in Bitcoin is not growing despite its increasing popularity over time. Instead
most users run a light node, verifying only block headers but not transactions,
or an ultralight node verifying nothing and relying on trusted advice from a
trusted server. This undermines decentralization as most clients rely on trust
rather than independent verification. It also undermines performance: block size
1
(and therefore transaction throughput) is artificially capped in part to mitigate
the burden of verification.

Figure 1: Growth of the Bitcoin blockchain over time, in GB. Source: www.
blockchain.com.
![GitHub Logo1](/Images/1.png)
<br>
Figure 2: Estimated number of full nodes participating in the Bitcoin and
Ethereum networks over time. Source: www.bitnodes.earn.com and www.
Ethernodes.org.
<br>
![GitHub Logo2](/Images/2.png)

In this work, our goal is to design a decentralized payment system that
offers efficient verification of system history from genesis without relying on
any external advice. Specifically, we aim to provide verification time constant
(푂(1)) in the number of transactions; we call such a blockchain, a general
blockchain.
We achieve this goal by including general proofs of state validity in each
block. 

Smart contract platforms and cryptocurrencies have captured mass attention but still have not been able to achieve mass adoption due to scalability and user experience issues. Even on Ethereum, which is the most widely used smart contracts platform, there have not been many examples of DApps which have seen mass adoption. There have been a few cases where one or the other particular application temporarily succeeded in achieving a significant user base, but it led to crippling of the entire network during the high network load times. Essentially this means that even the most advanced and widely used platforms are not ready for mass adoption yet.
<br><br >
The lightweight Earthchain network will strive to solve the scalbility and usability issues, while not taking any shortcut to compromise on decentralization and leveraging the existing developer community and ecosystem.
It will be a very powerful and scalable blockchain that will provide scalability and superior user experience to DApps/user functionalities.
<br/><br/>
On the other hand, there are a few smart contract platforms which boast of higher transaction throughput, but they compromise on decentralization in order to improve transaction speeds. Also, many of the upcoming solutions propose developing their own blockchains, neglecting the billions of dollars of market cap that DApps and other projects have already created on platforms like Ethereum and others. More importantly, they neglect the massive developer community and developer ecosystem that currently exists on platforms like Ethereum.
<br><br >
<b>The Herophilos development team has chosen to develop the first industrial decentrantralized platform that will have scalability and a working implementation very soon on the test network.</b> 

We expect to reduce the transfer time to 0, exchange and conversion of digital assets (e.g. crypto tokens) and cryptocurrencies in the future. 

Herophilos Limited has the intention to provide Earthchain wallet, payment API's and SDK's, products, identity solutions and other enabling solutions that will allow developers to design, implement DApps .The most important key pillar that lives at the foundation of Earthchain is the improvement of user experience, this representing a very undeveloped area of Blockchain applications. The Herophilos team plans to build high quality user experience Mobile/Web Browser libraries which will enable businesses to create real world end user applications on a large scale. In our development RoadMap of our industrial blockchain network will include supporting cross-chain transfers and third-party Decentralized exchanges, liquidity pools, etc. 

## Why should you chose Earthchain? 

Decentralized Apps are being proposed in large numbers, but the current blockchain ecosystem is not prepared to scale to match the demands of end user applications with mass adoption. Moreover the user experience of DApps is very poor and in no way conducive for average users. Slow block confirmations, high transaction fees, low scalability and poor user experience are some of the key roadblocks for the mass adoption of blockchain applications. The following section explains the problems prevailing in the current blockchain ecosystem and how the Matic Network intends to solve them. **Detailed technical specification are provided in the further sections of the white paper.**

### Slow Transactions {#tbd variable}

Blockchain transactions are typically very slow and have a very limited throughput. Most PoW ([Proof-of-Work](https://en.wikipedia.org/wiki/Proof-of-work_system)) based blockchain protocols have a limit on the block size and it takes a certain amount of time to generate a block. Each transaction also has to wait for multiple block confirmations due to potential chain re-organizations.<br/>

PoS ([Proof-of-Stake](https://github.com/ethereum/wiki/wiki/Proof-of-Stake-FAQs#what-is-proof-of-stake)) based blockchains try to counter these limitations using a staking mechanism, but the blockchains that are able to achieve high throughput with PoS are able to do so at the cost of decentralization. These limitations are often a necessary condition for public blockchains to ensure security and decentralization where a block needs to be propagated through the network and validated by all the nodes to achieve finality.<br/>

Earthchain solves this problem by using a high throughput blockchain with consensus provided by a selected set of Block Producers, chosen for every checkpoint by a set of Stakers. It then uses a Proof Of Stake layer to **validate the blocks and publish periodic proofs (merkle roots) of the blocks produced by the Block Producers to the Earthchain mainchain. This helps in achieving high level of decentralization while maintaining an extremely fast (< 1 seconds) block confirmation times.**

### Low Transaction Throughput {#tbd variable}

Public blockchains have to maintain a certain amount of time lag between the production of adjacent blocks so as to ensure ample time for block propagation. Also, the block size needs to be small so as to ensure quick propagation of the block through the network. This entails that the number of transactions in a particular block need to be fairly limited.<br />

Earthchain solves this problem by using a **worker node layers to produce the blocks.** Worker Nodes enable the system to produce blocks at a very fast rate. The system ensures decentralization using PoS checkpoints which are pushed to the Mainchain (Ethereum serves as the mainchain for a start).**This enables The Matic Network to theoretically achieve up to $$1^{16}$$  transactions per second on a single side chain.**

### Scalability {#tbd variable}

As discussed in the previous section, The Earthchain Network easily achieves a theoretical speed of up to $$1^{16}$$ transactions per second on a single side chain. **In future, The Earthchain Network is expected to be able to easily add more side chains verticaly by using Kubernetes containers to ramp up and down depending on the load to sustain and increase the total number of transactions on the Earthchain while using the same decentralized PoS layer.**


Theoretically the Earthchain Network has the capacity for 10 millions transactions per second with the usage of multiple side chains. Also, the mechanism to do so will be been demonstrated with the first Earthchain proof-of-concept with the first Earthchain side-chain and new chains can be added in due course of time.

### Size of Blockchain {#tbd variable}

Each block on the blockchain and/or compute state in case of a smart contract based blockchain must be validated by multiple nodes. Each node has to manage a copy of the state and the blocks. While the chain increases in size as the days go by, maintaining and validating the whole blockchain becomes difficult and results in fewer full nodes in public blockchains, which poses a risk for decentralization.<br/>

For the EarthChain Network, the primary layer which provides decentralization may choose to store only the blocks of Earthchain from the previous checkpoint to the next checkpoint. All previous transaction/block proofs have been submitted to the mainchain. **This enables extremely low fidelity PoS nodes which can be run in very low-cost machines with low storage. In future, The Earthchain Network intends to enable mobile device based PoS miners too. Our aim is to create the perfect size for blocks in order for Earthchain to provide low syncronisation time and also **

### Multiple micropayment channels with other off-chain solutions {#loooong}

Some payment channel solutions have proposed solutions to solve the problem of micro-payments. However, the process of opening and managing channels with multiple DApps or users is complex. Additionally, the speed and convenience of mediated payments over channels is still up for debate.

Since **The EarthChain Network uses a state-based architecture on an EVM (Earthchain Virtual Machine), it does not require payment channels to be opened between two parties. In fact, any valid Bitcoin address is a valid Earthchain Address and a receiver does not need to be on the Earthchain to receive payment. They would only need to have a Earthchain Wallet when they want to retrieve the payments on the main chain or spend it in the ecosystem on the Earthchain Network.**

### High Transaction Fees {#tbd variable}

With the rapid growth of the blockchain ecosystem, new crypto assets are increasingly being created, transferred, and sold, often involving multiple crypto tokens. Also, most decentralized apps have their own token and economy. Paying tokens for the services or doing any kind of transaction on blockchains requires on-chain transfers. Every blockchain has a transaction cost structure. For example, Ethereum charges gas fees on each transaction.

The amount of fees is an important factor to incentivize validators and prevent certain kinds of security attacks such as DoS. However, there is the problem of variation of fees (Depending upon the pending transaction pool) due to the limited block size.

**The Earthchain Network enables low cost transactions through achieving economies of scale by doing a large number of transactions on the general layer which ensures low cost, and then subsequently batching the proofs of the Earthchain blocks using the Merkle root of the blocks** to a highly decentralized mainchain (for ex. Ethereum) using a decentralized layer of PoS Stakers.

### Poor Usability {#tbd variable}

User interactions on DApps are often poor compared to their centralized counterparts. For the Decentralization revolution to achieve mass adoption, the user experience of DApps has to be on par with, if not better than, their centralized counterparts.

The Earthchain Development team is expected to work on various Mobile and Web browser integration tools and is pioneering protocols in this domain. It intends to build a ubiquitous mobile/browser app, which will act as a secured interaction layer for blockchain interactions. The Earthchain Development team will be publishing the designs and prototypes of these soon.


# Introducing the Earthchain Network

 As discussed in brief in the section above, the Earthchain Network aims to solve the problems faced by the blockchain ecosystem through building a decentralized platform using an adapted version of Python & Django Web framework togheter with ReactJS. This provides for fast and extremely low cost transactions with finality on a mainchain. The current working Testnet and alpha-Mainnet of the Earthchain Network works with Earthchain as a mainchain. <br/>

# Architecture 

Since the Earthchain Network's core focus is on mass user adoption, it is ideal that a deep dive into the Matic Network's technical architecture should start from a user journey.

When a user is transferring ETH or ERC20 tokens on the Ethereum network, they have to wait for the confirmation of the block which ranges from 14 seconds to 20 seconds. Even then the users have to wait for multiple block confirmations to be sure of the finality of the transaction. Let’s say you are buying a coffee or paying tokens to watch a movie. On each transaction you are not only paying a high fee, but also waiting for it to be confirmed. That serves as a deterrent for users wanting to use the service.

Moreover, during peak loads, a large number of transactions clog the Ethereum network and gas fees increase on each transaction in order to obtain faster confirmations. The Matic Network is proposed as a solution to overcome these problems.

Here is how the Matic Network will function: <br/>

1. A user deposits a cryptographic asset in the Matic contract on the mainchain (currently implemented with Ethereum blockchain only).
2. Once deposited, tokens get confirmed on the main chain, tokens will appear on the Matic Chain using Matic Deposit bridge (technical details explained in a dedicated section below).
3. The user can now transfer tokens to anyone they want almost instantly (Matic Chain has faster blocks - approximately 1 second or less) for almost negligible fees.
4. Whenever the user wishes to, they can withdraw tokens to the main Ethereum chain by establishing proof of remaining tokens on Root contract (contract deployed on Ethereum chain).

The same method will work for any ERC-20 token or other fungible crypto assets on the Ethereum blockchain.
The Matic Development Team has already created a demo version, available at: https://github.com/maticnetwork/contracts.

We expect the alpha version of the mainnet to go live very soon.
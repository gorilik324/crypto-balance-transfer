# Architecture of Web 3.0

Web3 is the future of the internet and its architecture differs greatly to its predecessor, web2. Let’s take Twitter, a Web2 application, as an example 
and look at its architecture

**Database:** Stores data such as users, posts, tags, and comments.

**Frontend End:** Frontend development handles the design and interface of the web application.

**Backend End:** backend development focuses on what happens behind the scenes, which defines the business logic. ie. login logout, posting etc

Thus, when a users publishes a tweet on Twitter, the essential are 

Interaction with its frontend / backend / database
All business logic (code) is hosted on centralized servers (AWS, Azure)
User interact with the website via internet browser
This is a simple example of how Web2 applications work today.


![1657833294712](https://user-images.githubusercontent.com/64011971/227530023-a7b4236f-a2cd-471a-b543-9b3dc6b375b8.jpeg)

However, everything changes with web3!

### Introduction to Web3 Application 

The fundamental concept of the entire process is straightforward. In essence, Web3 refers to an application that employs a decentralized network. This 
implies that the internet is being transformed into a new infrastructure based on blockchain technology. Web3 represents the new era of web development 
that empowers users to take charge of their data privacy and ownership instead of relying on third parties such as Twitter.

Let us delve into some basic terms:

**Web3** operates on permissionless blockchains, and its technologies form the basis for peer-to-peer (P2P) transactions, payments, services, and 
marketplaces.

**Blockchain** technology enhances the way data is collected and managed across the internet. It brings together valuable data through the use of 
Artificial Intelligence (AI) and Internet of Things (IoT). Additionally, data stored on blockchain is immutable and cannot be tampered with.

A **dApp** is a decentralized application that operates on a blockchain or P2P network of computers. It enables users to participate in transactions 
directly with each other, eliminating the need for a central authority.

Architecture of a Web3 application

![1657833328873](https://user-images.githubusercontent.com/64011971/227531091-76da167a-5d12-43f3-8203-094059e44c0f.jpeg)


### An Overview
Let’s explore the whole process of what makes Web3 different.

**1. Blockchain** 

These refer to globally accessible state machines that are upheld by a network of peer-to-peer nodes. In summary, they are state machines that can be 
written and accessed by anyone worldwide. Nonetheless, while users can append new data to the blockchain, they are unable to modify existing data.

**2. Smart Contracts**

Smart contracts are business logic that is stored on a blockchain (state machines) and can be programmed to execute when certain predetermined 
conditions are met, without requiring the involvement of intermediaries.

The most widely recognized Smart contracts at present are transaction protocols that operate on the Ethereum blockchain. They are typically scripted in 
high-level languages such as Solidity, which specifies the logic underlying state changes. Smart contracts operate exclusively on private peers owned by 
particular network members, processing verified data that is hosted by those peers.

**3. Ethereum Virtual Machine (EVM)**

These machines’ purpose is to carry out the logic defined in the smart contracts. They handle the state changes that occur on the state machine.

**4. Front End process**

It enables users to connect and submit requests for contract function calls via the application's frontend, thereby facilitating communication with the 
application logic specified in smart contracts.

### Comparing Web2 and Web3 Frontend

In Web2, the application frontend allows users to query and post to the database, and this remains unchanged in Web3. Consequently, the primary 
responsibilities of a Web3 frontend developer are similar to those of their Web2 counterparts, as they are responsible for implementing all the features 
that users interact with. Typically, Web3 frontend developers require the same skill set, which includes expertise in HTML, CSS, JavaScript, React.js, 
and other relevant tools.

The significant difference, however, lies in the use of Web3.js, which is a suite of JavaScript libraries that enables interaction with an Ethereum 
node. Essentially, Web3.js provides an API that facilitates communication with the blockchain node using either a HTTP or IPC connection.

### How to interact with the Ethereum Virtual Machine (EVM) & Smart contracts.

For a Web3 application (dApp) to function properly, it must either host an Ethereum node or employ the services of a third-party provider such as 
Infura, Alchemy, or Quicknode. This is crucial because any node can execute a transaction or query data on the Ethereum Virtual Machine. However, it's 
worth noting that running a complete Ethereum node can be expensive and time-consuming to maintain. Consequently, relying on a third-party service may 
be a more practical option.

Moving on, we will discuss "Web3 providers," which enable interaction with the Ethereum Virtual Machine and smart contracts.

![1657833427743](https://user-images.githubusercontent.com/64011971/227540745-2ef6a556-69da-4308-a657-bbf5027fa0fb.jpeg)


Ethereum providers implement JSON-RPC specifications to facilitate communication with blockchain networks. Remote Procedure Call (RPC) is a request-
response protocol that outlines the procedures for a client to send a message to a remote machine to execute a function and retrieve a response. In this 
communication, the program runs on the client machine, with the client having no knowledge of the remote machine. All communication occurs via HTTP or 
Web Sockets.

Unlike centralized databases that grant access to apps through logins, dApps authenticate access via a web3 provider. Providers like Metamask, a 
cryptocurrency wallet, act as transaction signers and providers. It stores encrypted private keys using the browser's data storage. Write requests and 
transactions are signed with the client's private key, with each transaction incurring a fee in Ethereum, which goes to other nodes (miners) that verify 
the transactions.

![1657834310341](https://user-images.githubusercontent.com/64011971/227541259-09f203d2-ebad-4cc7-bb57-445f16af0e2f.jpeg)


When a user wants to create a new transaction, the dApp, through the web3 provider, will prompt the user to sign the transaction using their 
private key. After the user has signed, the dApp will interact with the smart contract on behalf of the user and broadcast the output to the Ethereum 
network.

### Storage on the Ethereum Blockchain

Both IPFS and Swarm are decentralized off-chain storage solutions that can be used to store data and files for dApps, as storing 
everything on the Ethereum blockchain can become extremely expensive due to the associated transaction fees. IPFS uses content-addressing to identify 
each file in a global namespace connecting all computing devices, while Swarm is designed specifically to provide permissionless, censorship-resistant 
infrastructure for the deployment of dApp code. Providers like Infura or Pintara can be used to pin files to IPFS and store them on the blockchain, 
while Swarm has its own built-in incentive system for users to store and distribute data on the network.

![1657837304552 (1)](https://user-images.githubusercontent.com/64011971/227541633-d08efe45-dc4b-46ad-bef3-247797586335.jpeg)


Another option is cloud servers, Azure or AWS. However, that would resemble Twitter's web2 architecture, where we have the centralization of data. In 
addition, if Azure or AWS were to go down, censor your app, you would no longer have access to the data. For the above reasons, a genuine dApp would 
store all of its off- chain data on a decentralized storage option.

### Wrapping up 

Blockchain technology will continue to play an essential role in internet infrastructure as Web3 evolves. Web3 is a shift in the paradigm, where the 
users gain control of their privacy and data. It will also be interesting to see how Big tech companies will react to this future trend.



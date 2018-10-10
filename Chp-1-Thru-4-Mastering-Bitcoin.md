# What Is Bitcoin? Chp 1.

Bitcoin is a collection of technologies that form a basis of a digital money ecosystem. It's units of currency call Bitcoin that's used to store and transmit value amoung participanta in the bitcoin network. It takes the place of fiat currency. 

Behind the scenes, bitcoin is also the name of the protocol, a peer-to-peer network, and a distributed computing innovation. The bitcoin currency is really only the first application of this invention. Bitcoin represents the culmination of decades of research in cryptography and distributed systems and includes four key innovations brought together in a unique and 
powerful combination. Bitcoin consists of:

1. A decentralized peer-to-peer network (the bitcoin protocol)
2. A public transaction ledger (the blockchain) 
3. A set of rules for independent transaction validation and currency issuance
   (consensus rules)
4. A mechanism for reaching global decentralized consensus on the valid           blockchain (Proof-of-Work algorithm).

## History of Bitcoin

Bitcoin was invented in 2008 with the publication of a paper titled "Bitcoin: A Peer-to-Peer Electronic Cash System, written under the alias of Satoshi Nakamoto.
The bitcoin network started in 2009, based on a reference implementation published by Nakamoto and since revised by many other programmers. The implementation of the Proof-of-Work algorithm (mining) that provides security and resilience for bitcoin has increased in power and now exceeds the combined processing power of the world’s top supercomputers.      

Satoshi Nakamoto withdrew from the public in April 2011, leaving the responsibility of developing the code and network to a thriving group of volunteers. The identity of the person or people behind bitcoin is still unknown. However, neither Satoshi Nakamoto nor anyone else exerts individual control over the bitcoin system, which operates based on fully transparent mathematical principles, open source code, and consensus among participants.

## Questions: 
             Will Bitcoin ever be asset backed?

             Once Bitcoin has reached its limits, what will the cost of goods and services be?

             Will Central Banks really go away?

# How Bitcoin Works  Chp 2.

The bitcoin system is based on decentralized trust. Instead of a central trusted authority, in bitcoin, trust is achieved as an emergent property from the interactions of different participants in the bitcoin system. Bitcoin uses a key system to activate a contract. This key system consists of a Public and Private key. The public key is used to transact business and the private key is use to store the value the contract produced. 

## Bitcoin Transactions

A bitcoin transaction tells the network that the owner of some bitcoin value has authorized the transfer of that value to another owner. The new owner can now spend the bitcoin by creating another transaction that authorizes the transfer to another owner in a chain of ownership.

Transaction Inputs and Outputs

Each transaction contains one or more "inputs," which are like debits against a bitcoin account. On the other side of the transaction, there are one or more "outputs," which are like credits added to a bitcoin account. The inputs and outputs differ slightly. The outputs are less because a fee is attached to it.

The transaction also contains proof of ownership for each amount of bitcoin (inputs) whose value is being spent, in the form of a digital signature from the owner, which can be independently validated by anyone. In bitcoin terms, "spending" is signing a transaction that transfers value from a previous transaction over to a new owner identified by a bitcoin address.

## Making Change

Many bitcoin transactions will include outputs that reference both an address of the new owner and an address of the current owner, called the change address. This is because transaction inputs, like currency notes, cannot be divided. 
An example of this would be, say you went to the store and you bought something that cost a dollar and you gave the store clerk a 5 dollar bill. You would get 4 dollars back.

The same concept applies to bitcoin transaction inputs. If you purchased an item that costs 5 bitcoin but only had a 20 bitcoin input to use, you would send one output of 5 bitcoin to the store owner and one output of 15 bitcoin back to yourself as change (less any applicable transaction fee). 

## Questions:

1. Would it be better to just send 5 bitcoin and not have to make 2 transactions?
2. If you have a wallet on your desktop what would stop a hacker from entering your wallet?

# Bitcoin Core Chp 3.

Bitcoin is an open source project and the source code is available under an open (MIT) license, free to download and use for any purpose. Open source means more than just free to use. It also means that bitcoin is developed by an open community of volunteers. By 2016, bitcoin’s source code had more than 400 contributors with about a dozen developers working on the code almost full-time and several dozen more on a part-time basis. 

When bitcoin was created the software was actually completed before the whitepaper was written. Satoshi wanted to make sure it worked before writing about it. That first implementation has been heavily modified and improved. It has evolved into what is known as Bitcoin Core. Bitcoin Core implements all aspects of bitcoin, including wallets, a transaction and block validation engine, and a full network node in the peer-to-peer bitcoin network.

## Bitcoin Development Environment

If you’re a developer, you will want to set up a development environment with all the tools, libraries, and support software for writing bitcoin applications. In this highly technical chapter, we’ll walk through that process step-by-step. If the material becomes too dense (and you’re not actually setting up a development environment) feel free to skip to the next chapter, which is less technical.

## Running a Bitcoin Core Node

Bitcoin’s peer-to-peer network is composed of network "nodes," run mostly by volunteers and some of the businesses that build bitcoin applications. Those running bitcoin nodes have a direct and authoritative view of the bitcoin blockchain, with a local copy of all the transactions, independently validated by their own system. By running a node, you don’t have to rely on any third party to validate a transaction. Moreover, by running a bitcoin node you contribute to the bitcoin network by making it more robust.

Running a node, however, requires a permanently connected system with enough resources to process all bitcoin transactions. Depending on whether you choose to index all transactions and keep a full copy of the blockchain, you may also need a lot of disk space and RAM. As of early 2018, a full-index node needs 2 GB of RAM and a minimum of 160 GB of disk space. That's a lot of memory for a PC.

## Bitcoin Core Application Programming Interface (API)

The Bitcoin Core client implements a JSON-RPC interface that can also be accessed using the command-line helper bitcoin-cli. The command line allows us to experiment interactively with the capabilities that are also available programmatically via the API. 

Exploring Blocks

Commands: getblock, getblockhash

Exploring blocks is similar to exploring transactions. However, blocks can be referenced either by the block height or by the block hash.

## Using Bitcoin Core’s Programmatic Interface

The bitcoin-cli helper is very useful for exploring the Bitcoin Core API and testing functions. But the whole point of an application programming interface is to access functions. Bitcoin Core’s API is a JSON-RPC interface. JSON stands for JavaScript Object Notation and it is a very convenient way to present data that both humans and programs can easily read. RPC stands for Remote Procedure Call, which means that we are calling procedures (functions) that are remote (on the Bitcoin Core node) via a network protocol. In this case, the network protocol is
HTTP, or HTTPS (for encrypted connections).

## Questions:

1. If you copy Bitcoin Core to your local drive will the blockchain get to large for your PC?
2. Can the Blockchain be used for more than just transactions?

# Keys & Addresses Chp 4.

Bitcoin is based on cryptography, which is a branch of mathematics used extensively in computer security. Cryptography means "secret writing" in Greek, but the science of cryptography encompasses more than just secret writing, which is referred to as encryption. Cryptography can also be used to prove knowledge of a secret without revealing that secret (digital signature), or prove the authenticity of data (digital fingerprint).

These types of cryptographic proofs are the mathematical tools critical to bitcoin and used extensively in bitcoin applications. Encryption is not an important part of bitcoin, as its communications and transaction data are not encrypted and do not need to be encrypted to protect the funds. In this chapter we will introduce some of the cryptography used in bitcoin to control ownership of funds, in the form of keys, addresses, and wallets.

Ownership of bitcoin is established through digital keys, bitcoin addresses, and digital signatures. The digital keys are not actually stored in the network, but are instead created and stored by users in a file, or simple database, called a wallet. The digital keys in a user’s wallet are completely independent of the bitcoin protocol and can be generated and managed by the user’s wallet software without reference to the blockchain or access to the internet. Keys enable many of the interesting properties of bitcoin, including decentralized trust and control, ownership attestation, and the cryptographic-proof security model.

Most bitcoin transactions require a valid digital signature to be included in the blockchain, which can only be generated with a secret key; therefore, anyone with a copy of that key has control of the bitcoin. Keys come in pairs consisting of a private (secret) key and a public key. Think of the public key as similar to a bank account number and the private key as similar to the secret PIN, or signature on a check, that provides control over the account. 

In the payment portion of a bitcoin transaction, the recipient’s public key is represented by its digital fingerprint, called a bitcoin address, which is used in the same way as the beneficiary name on a check. In most cases, a bitcoin address is generated from and corresponds to a public key. However, not all bitcoin addresses represent public keys; they can also represent other beneficiaries such as scripts.

## Public Key Cryptography and Cryptocurrency

 Public key cryptography was invented in the 1970s. Since the invention of public key cryptography, several suitable mathematical functions, such as prime number exponentiation and elliptic curve multiplication, have been discovered. These mathematical functions are practically irreversible, meaning that they are easy to calculate in one direction and infeasible to calculate in the opposite direction. Based on these mathematical functions, cryptography enables the creation of digital secrets and unforgeable digital signatures. Bitcoin uses elliptic curve multiplication as the basis for its cryptography.

In bitcoin, cryptography was used to create a key pair that controls access to bitcoin. The key pair consists of a private key and—derived from it—a unique public key. The public key is used to receive funds, and the private key is used to sign transactions to spend the funds.

There's a process between the public and private keys that allows the private key to be used to generate signatures on messages. This signature can be validated againsnt the public key with out the private key being known.

The current bitcoin owner presents his public key and a signature (different each time, but created from the private key)which will allow him in a transaction to spend those bitcoin. Through the presentation of the public key and signature, everyone in the bitcoin network can verify and accept the transaction as valid, confirming that the person transferring the bitcoin owned the bitcoin at the time of the transfer.

## Private and Public Keys

A wallet contains a collection of key pairs, each consisting of a private key and a public key. The private key is a number picked at random. From the private key, the elliptic curve multiplication is used to generate a public key. From the public key a one-way cryptographic hash function is used to generate a bitcoin address.

## Question:

              Is the private key only numerical or is it alphanumeric? 









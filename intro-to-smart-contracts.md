# Introduction to Smart Contracts

This segment primarily deals with Solidity. A contract in the sense of Solidity is a collection of code (its functions) and data (its state) that resides at a specific address on the Ethereum blockchain. 

A blockchain is a globally shared, transactional database. This means that everyone can read entries in the database just by participating in the network. If you want to change something in the database, you have to create a so-called transaction which has to be accepted by all others.

## The Ethereum Virtual Machine

The Ethereum Virtual Machine or EVM is the runtime environment for smart contracts in Ethereum. It is not only sandboxed but actually completely isolated, which means that code running inside the EVM has no access to network, filesystem or other processes. Smart contracts even have limited access to other smart contracts.

## Installing the Solidity Compiler

Versioning

Solidity versions follow semantic versioning and in addition to releases, nightly development builds are also made available. The nightly builds are not guaranteed to be working and despite best efforts they might contain undocumented and/or broken changes. Using the latest release is recommended.

## Remix

Remix is recommended for small contracts and for quickly learning Solidity.

You can access Remix online, you don’t need to install anything. If you want to use it without connection to the Internet, go to https://github.com/ethereum/browser-solidity/tree/gh-pages and download the .ZIP file as explained on that page.

## npm / Node.js

Use npm for a convenient and portable way to install solcjs, a Solidity compiler. The solcjs program has less features than all options further down this page. The Using the Commandline Compiler documentation assumes you are using the full-featured compiler, solc.

## Question:

         How would you connect your code to the solcjs complier?
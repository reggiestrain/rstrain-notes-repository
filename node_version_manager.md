# My Node Version Manager File

## $ nvm -h

# Running version 1.1.6.

# Usage:

##   nvm arch 
                      : Show if node is running in 32 or 64 bit mode.
##  nvm install <version> [arch]
                      : The version can be a node.js version or "latest
                      " for the latest stable version.
                      Optionally specify whether to install the 32 or
                      64 bit version (defaults to system arch).
                      Set [arch] to "all" to install 32 AND 64 bit ve
                      rsions.
                      Add --insecure to the end of this command to by
                      pass SSL validation of the remote download server.
##  nvm list [available]
                      : List the node.js installations. Type "available
                      " at the end to see what can be installed. Aliased as ls.
##  nvm on 
                      : Enable node.js version management.
##  nvm off 
                      : Disable node.js version management.
##  nvm proxy [url]   : Set a proxy to use for downloads. Leave [url] b
                      lank to see the current proxy.
                      Set [url] to "none" to remove the proxy.
##  nvm node_mirror [url] 
                      : Set the node mirror. Defaults to https://nodejs
                      .org/dist/. Leave [url] blank to use default url.
##  nvm npm_mirror [url] 
                      : Set the npm mirror. Defaults to https://github.
                      com/npm/npm/archive/. Leave [url] blank to default url.
##  nvm uninstall <version>
                      : The version must be a specific version.
##  nvm use [version] [arch]
                      : Switch to use the specified version. Optionally
                      specify 32/64bit architecture.
                      nvm use <arch> will continue using the selected
                      version, but switch to 32/64 bit mode.
##  nvm root [path] 
                      : Set the directory where nvm should store differ
                      ent versions of node.js.
                      If <path> is not set, the current root will be
                      displayed.
##  nvm version 
                      : Displays the current running version of nvm for
                      Windows. Aliased as v.

# Intro To Ethereum And Smart Contracts

## What is Ethereum?

  Basically, Ethereum is a database that is decentralized. A host of nodes(computers all over the world) that contain transactions that conduct business
  between people, between contacts, and between people and contracts. 

  The reason why Ethereum is decentralizied is because no one can change it, no one can see it, anyone can run it, and anyone can anonymously create on it. Also, in most cases it's pretty trustworthy. Currently the cost to compute is high.

## History of Ethereum

Bitcoin started the whole process back in 2008. The were many contributions made to Bitcoin by blockchain engineers and researchers. As Bitcoin grew it inspired developers and entrepreneurs to create decentralizied apps. However, a problem arose. Inside the Bitcoin community, they were all starting their own blockchains.
There was one innovative individual whose name was Vitalik Buterin who said, "Shouldn't there be one blockchain that everyone can build their decentralizied applications on?" and Ethereum was born. The Ethereum blockchain mimic's the Internet.   

The Ethereum Whitepaper

Vitalik published a white paper on Ethereum in late 2013. Many of the ideas and concepts were taken from Bitcoin. Vitalik wanted a more general purpose blockchain the could do everything that Bitcoin could do and more. 

Bitcoin vs Ethereum

Bitcoin has limitations. It doesn't have a general purpose programming language that "apps" can use to build decentralizied apps. Bitcoin's programming language is currently limited to the point it can't store state or loop through data. 

Other Differences

Bitcoin is capped at 21 million coins forever, ether has no limit. If one would say that Ethereum has any draw backs it would be that Ether has an annual ceiling of 18 million per year. Block rewards are different Bitcoin: 12.5 btc Ether: 5 eth. Block rates are different Bitcoin: 10 min. Ether: 15 sec.

## Ethereum In Depth

Is Ethereum the same as Ether?

No, it is not. Ethereum is the network and Ether is the "fuel" that powers the network. Ether is used to pay transaction fees, launch contracts, and call functions from contracts.

## Ethereum Virtual Machine

Ethereum is a network of computers. The EVM is the program that the network of computers. And what does the EVM run? Right, smart contracts. 

## Smart Contracts

You can use different languages such as Serpent, Viper, and Solidity to create your contracts. There are also lots of developer tools available. Smart contracts can store data or in developer terms, state. The code can manipulate data based on programming logic.

Deploying a smart contract

The process is as follow: a) write code, b) compile smart contract down to EVM bytecode, c) send bytecode as part of transaction to the network, and d) transaction gets put into a block and verified.

## Ethereum Yellow Paper

In 2014, ethereum yellow paper was released by co-founder Gavin Wood. It defined the technical specification of the EVM and how it would work.

what's gas?

Gas is the cost of invoking a smart contract method. Gas is a unit of measurement. It determines how much computation the EVM needs.

## What's an ethereum node?

A node is also called an ethereum client. Nodes/clients parse and verify the blockchain and its smart contracts and everything related. There are some nodes that only do wallets these types of nodes place their trust in services that do that for them.
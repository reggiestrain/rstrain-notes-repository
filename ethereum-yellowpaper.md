# The Ethereum Blockchain

Ethereum can be viewed as a transaction-based state machine: It began with a genesis state(or block) and incrementally execute transactions to morph it into some final state. The state can include such information as account balances,
reputations, trust arrangements, data pertaining to information of the physical world; just about anything that can be done on a computer. 

Transactions are collated into blocks; blocks are chained together using a cryptographic hash as a means of reference. Blocks function as a journal, recording a series of transactions together with the previous block and an identifier for the final state. 

Mining is the process of dedicating effort (working) to bolster one series of transactions (a block) over any other potential competitor block. It is achieved thanks to a cryptographically secure proof. This scheme is known as a proof-of-work.

## Value

In order to incentivise computation within the network, there needs to be an agreed method for transmitting value. To address this issue, Ethereum has an intrinsic currency, Ether, known also as ETH. The smallest subdenomination
of Ether, and thus the one in which all integer values of the currency are counted, is the Wei. One Ether is defined as being 10 to the 18th power Wei. 

## World State

The world state is a mapping between addresses (160-bit identifiers) and account states (a data structure serialised as RLP). Though not stored on the blockchain, it is assumed that the implementation will maintain this mapping in a modified Merkle tree. 

## The Block

The block in Ethereum is the collection of relevant pieces of information (known as the block header ), H, together with information corresponding to the comprised transactions. Information include:

parentHash: The Keccak 256-bit hash of the parent block’s header
ommersHash: The Keccak 256-bit hash of the ommers list portion of the block
beneficiary: The 160-bit address to which all fees collected from the successful mining of this block be transferred. Just to name a few.

## Gas and Payment

In order to avoid issues of network abuse and to sidestep the inevitable questions stemming from Turing completeness, all programmable computation in Ethereum is subject to fees. The fee schedule is specified in units of gas. Any given fragment of programmable computation (this includes creating contracts,
making message calls, utilising and accessing account storage and executing operations on the virtual machine) has a universally agreed cost in terms of gas.

Every transaction has a specific amount of gas associated with it and it's called gasLimit. This is the amount of gas which is implicitly purchased from the sender’s account balance. The purchase happens at the according gasPrice, also
specified in the transaction. The transaction is considered invalid if the account balance cannot support such a purchase.

## Questions:

        Can any cryptocurrency run on the Ethereum Blockchain?
        Who gets the sender's gas after the transaction?
        In mining who gets the bitcoin if you have two miners computate the hash at the same time?
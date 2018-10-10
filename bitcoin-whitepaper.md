# Bitcoin Whitepaper

Bitcoin was designed as a digital peer-to-peer electronic currency that allowed online transactions to be sent from one party to another. A method was created to link blocks of data together and each block had information from the previous to validate it. This was done using SHA256. This method also helped stop what is called "double-spending".

## Transactions

 An electronic coin as a chain of digital signatures. Each owner transfers the coin to the next by digitally signing a hash of the previous transaction and the public key of the next owner and adding these to the end of the coin. The payee can verify the signatures to verify the chain of ownership. 

Timestamping

Bitcoin uses a timestamp server. A timestamp server works by taking a
hash of a block of items to be timestamped and widely publishs the hash. The timestamp proves that the data must have existed at the time, surely, in order to get into the hash. Each timestamp includes the previous timestamp in its hash, forming a chain, with each additional timestamp reinforcing the ones before it.

To help timestamping work Proof-of-Work was established. The proof-of-work involves scanning for a value that when hashed, such as with SHA-256, the hash begins with a number of zero bits. The average work required is exponential in the number of zero bits required and can be verified by executing a single hash.

The Network

In order for the network to run properly it must have:

1) New transactions are broadcast to all nodes.
2) Each node collects new transactions into a block.
3) Each node works on finding a difficult proof-of-work for its block.
4) When a node finds a proof-of-work, it broadcasts the block to all nodes.
5) Nodes accept the block only if all transactions in it are valid and not already spent.
6) Nodes express their acceptance of the block by working on creating the next block in the chain, using the hash of the accepted block as the previous hash.

# Question:

          Could there be a time where the integrty of the nodes be compromised?
          
# TheBorneoEcosystem

The Borneo Ecosystem is a new project that takes advantage of modern cryptography, decentralized systems, and peer-to-peer networking. It uses Block Lattices, Pivots, Bridges, VMs, ICDs (Interconnected-Design), and more.

## Cryptography


* **Hash Function:** BLAKE2B

* **Digital Signature:** ED25519, Dilithium

* **Technology Used:** Verifiable Delay Functions (VDFs), Verifiable Random Functions (VRFs), Block Lattices


## BorneoLattice

**Includes:** Temp Lattice

A Block Lattice is constructed where each account has its own chain. This chain can be used to send, receive, setup, update.

The home of the information required for the account is found by `H(PK)` with the first block being a setup block.

### Setup Block

The setup block is the block that contains all the information related to the account. It contains the public key, rng, ecies block, and init information.

To setup a new chain or temp lattice, you can use the setup block. It can also be used for various other operations.

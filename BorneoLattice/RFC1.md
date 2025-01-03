# BorneoLattice

The BorneoLattice is a structure designed as a Directed Acrylic Graph (DAG), or more specifically, a Block Lattice, such as that used in nano, that uses the consensus mechanism of **Delegated Proof of Stake (DPOS)** and **Proof-of-Work (PoW)**.


## Root Chain (ALMAC)

It offers a `root chain`, the **Account Ledger Management Chain (ALMAC)** that is its own blockchain where only the user can sign. The root chain consists of data related to the address and initiating new chains. It also allows you to communicate directly with **GLCC**.

## General Ledger Contract Chain (GLCC)
It offers a `general contract chain`, the **General Ledger Contract Chain (GLCC)** where registration can occur. This registration usually takes a certain amount of proof-of-work to avoid using too many addresses.

### GLCC Types

It offers the `X59 Registar Chain` which is a RFC5280 approach to **Certificate Authorties and Intermediaries** done on a block lattice to register addresses with the main chain. It requires PoW to register an address. It is a subset of **GLCC**. This provides CAs to provide shorter chains of intermedieraries all registered under Certificate Authority using PoW.

It offers the `Bank Registar for Staking (BRFS)`, a way of including staking modules with gains stored in the Bank, delegated by Bank Stakers. This include Bank Stakers on the main chains with interconnectedability, and other modules for different banks. It includes currencies supported by banks, backed by staking of main currency.

It offers the `Database Registar`, for hosting content.

## ALMAC Account Sidechains (AccSidChains)

It offers `account sidechains`, the **Account Sidechains (ALMACside)** are useful for other activities. This includes general, actions, contracts, blocks (a special one-use block), access, among others.

### Types of AccSidChains

#### IMX

It offers `IMX Setup Block Chain`, the **Immutable Setup Block Chain (IMXSetupBL)**, where all is stored for each chain and can be gathered quite easily. This id's each block and creates a setup of sidechains with immutable information.

# ICDBridging

It provides interfaces to communicate with using **BorneoBridge (BB)** and **BorneoCrates (BorCrates)**. **BorneoBridge** is hard-built rules that must apply, while **BorneoCrates** is **ICD** (Interconnected-Design Interface) that can be defined through rules and structures. These definitions use `BorneoCrates Standard Library` and are defined in `BorneoCrates/..`

--

**Pivots** are extensively used to reduce storage size. A **PivotPoint** is any indepedent entity that forms its own `pivot`.

--

**BorWorkers** are used to do **tasks** that range from all types of different actions on the lattice. This can include pruning, validating, relaying, serving, initializing, and keeping the ecosystem running.

--

**IMXSetup Blocks (IMXb)** are immutable-setup blocks.

# Future

- Register-Based Virtual Machine

## Account Sidechains

* [0x00] General (Payment, Voting,
* [0x01] Account Blocks
* [0x02] Domain Block

## Cryptography Used:

* [Hash] BLAKE2B(key,40)
* [Hash] BLAKE3
* [Signature] ED25519

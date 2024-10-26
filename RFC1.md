# RFC#1: BorneoCrateRepoSystem

The **BorneoCrateRepoSystem** consists of which crates are valid for a certain block lattice, or chain. It uses the `BorneoCrateRootPivot (BCRP)` which is a label or PivotPoint using a 20-byte digest encoded in hex derived from the public key.

It consits of a borneo rust standard library for defining new **BorneoCrates** and **BorneoLibraries**.

## BorneoCrateRootPivot

There are a the majority of designed ones located under the name `generic`.

There are other labels too, such as `centralized`, `centralized-std`, `centralized-[id]`, `open`, `private`, `col-[hex]` (for collection)




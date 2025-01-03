# RFC1.1: Account Ledger Management Chain (ALMAC) Root

The ALMAC serves as the core component to the chain.

## ALMAC Genesis Block

### Header

```yaml
BLOCK-HASH: EB9B0F9B83DD764A2D862171B1810C519B8A1C5DFF5AA693C51D3DB8F4B801DF
[Optional] Authority-Signature: <insert signature>
```

### BLOCK

```yaml
id (u64): 0
BorneoAccount (BLAKE2B ENCODED IN BASE32): BA9_TGJX7DTLG5D3FK2VLUY6CC2O775EJLQHF33QHPCJRO2Z26LIFR3Q
PublicKey (ED25519): 1E9D38B5274152A78DFF1A86FA464CEADC1F4238CA2C17060C3C507349424A34
Link-Hash (Hash-of-PK For Genesis): A72C87777B2E4D542B26A2FE94E985F081C0489996CFA8210240A3EBC2C87621
To-Account: Self
Nonce (u64): 340
Acc Type (u16): 0
Tx Type (u16): 0

Container Meta: <Container Metadata>
Container Contents: <Container Contents>

Hash-of-Contents (HoC): 643F5BBE916FF786BCE43264D02CE05B1B1513D953F41E2D5CB5D25319E9811C
Digital-Signature (ED25519 of HoC): <insert digital signature>
```

## ALMAC TYPES

### 0x00: Payment Ledger

The payment layer works as an easy-to-use basic payment ledger with send and receive blocks

### 0x01: Voting Ledger

A voting ledger for voting in delegates. You can also access delegates by sending a transaction to be a part of their DelegateSumatraChain.

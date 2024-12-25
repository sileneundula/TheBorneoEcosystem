# Talkr

**Talkr** is a way of communicating with certain blocks off-chain and in a simple manner.

## How It Works

1. The input (bytes) to Talkr is hashed By Blake2b(48)
2. It is then encoded in Base58 with the `TALKR_` prefix

## What It Does

It allows a general consensus point at which one can interact with others.

## Storage

All storage is kept by a DHT or in blocks.

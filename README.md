# SlinkyRFCs

## Description

**SlinkyNet** is a novel construction of a decentralized, open, peer-to-peer network for a new internet age called `SlinkyNet`. It is inspired by Freenet, I2P, Tor, Zeronet, and GNUnet among others. It is a layered internet with Slinky being layer 1 and offering many protocols to support it. It is seperate from the usual internet and works in different ways, seperating it as a different project with its own ecosystem.

It is written in pure-rust using the `libp2p` and `tokio` library with custom protocols as well as access to different resources like block lattices (DAG) for services, srvless logic, and overlay networks for anonymity.

## Philosphy

Slinky supports the right to privacy, security, anonymity (in some cases), and focuses on being easy for the client to use, with more advanced features customizable.

## Features

### SlinkyL1: Layer 1 Solution To A Peer-To-Peer Network

[[Library] libslinkynet](https://github.com/sileneundula/libslinkynet)

Layer 1 is the basis of the network, called a **swarm**, of peer-to-peer hosts who send messages through custom protocols. Slinky offers this as the basis and it is the widely used network, while offering other options like an overlay network and layer 2 options. It relies on [TheBorneoEcosystem](https://github.com/sileneundula/TheBorneoEcosystem) for transactions, logic, and services.

It also offer **Bridges** to services which use **Directed Acyclic Graph (DAG)**.

#### TheBorneoEcosystem: A Block Lattice For The Future

[[RFCs] TheBorneoEcosystem](https://github.com/sileneundula/TheBorneoEcosystem)

[[Library] libborneo](https://github.com/sileneundula/libborneo)

**SlinkyL1** relies on libborneo (soon to be renamed) as a block lattice to introduce many features to the network. These includes new lattices introduced by `Init-Chain`, blocks of data created by `Init-Block`, and voting schemes to choose delegates. It also includes the **X59 Cert Authority System** for certificates for a transparent certificate system.

**TheBorneoEcosystem** can be quite complicated and is divided into smaller pieces to make it easier to download pieces of the chain without having to download the entire chain.

Workers and Services are employed to ensure tasks be done which may include **incentives**.

#### LamentSearch

An indexing mechanism that offers ways of customizing tags and keywords for finding data through a stricter search way that is efficient.

## How It Works

The simple idea of Slinky is that it is peer-to-peer at layer 1. It is designed as a new internet seperate from the other internet with special functions and custom protocols to make it easy for peers to interact with each other.

### How Peer Discovery Works

**Peer Discovery** is done using the Kademelia DHT protocol to find peers. This offers a decentralized approach to finding nodes derived from their public key.

**Cryptography Note:** It derives its keypair from ED25519, ECDSA, or SECP256k1, ED25519 being the default. It will also most likely support RSA.

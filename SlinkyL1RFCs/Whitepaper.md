# SlinkyNet: A Novel, Layer-1, Decentralized, Peer-To-Peer Network That Interacts With The BorneoEcosystem To Deliver A New Internet Experience Seperate

**Author:** `silene`

**Timestamp:** 14 Dec 2024

## Abstract

SlinkyNet is a **Layer-1, Peer-To-Peer Network** that interacts with the **libborneo**, a block lattice that uses DPOS for consensus, to deliver a new experience seperate from other projects. It uses custom protocols to interact with the network and relies on a block lattice for many tasks and transactions. This block lattice uses ALMAC, a method of generating new chains seperate from other chains as described in the ALMAC block. This reduces the number of chains that have to be received.

The basis of SlinkyNet is setting up a decentralized network that offers features like serverless logic, a Public-Key Infrastructure (PKI), and other advanced features. It uses the Kademilia DHT protocol for peer discovery, thus offering many advances over mDNS.

## 1. The Slinky Peer-To-Peer Network

The Slinky Peer-to-Peer Network is written in Rust and uses the library `libp2p` and `tokio`. It offers fast speeds, secure code, and many other features like custom protocols, routing, and overlay networks.

## 2. Transport

There are two main transports that can be used in the SlinkyNetwork. These are:

* SlinkyTransportTCP
* SlinkyTransportWSS

They both offer **yamux multiplexing**, offering scalability over a single tcp connection.

Noise encryption is used using the public key to authenticate and generating ephermal keys for each connection.

## 3. Security

Slinky offers security through **Noise** as opposed to **TLS**.

### Cryptography

It uses ED25519 by default, but can also use SECP256k1 and ECDSA. The PeerID is derived from the public keys of these keys. These are usually ephermal keys that are generated each time, although static keys can also be used in certain situations.

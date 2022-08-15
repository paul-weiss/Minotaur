# Minotaur

Welcome! This is the repository for the implementation of the Minotaur consensus protocol.

## Paper

__[Minotaur](https://arxiv.org/pdf/2201.11780.pdf): Multi-Resource Blockchain Consensus__ (to appear in ACM CCS 2022)

Abstract: 
Resource-based consensus is the backbone of permissionless distributed ledger systems. The security of such protocols relies fundamentally on the level of resources actively engaged in the system. The variety of different resources (and related proof protocols, some times referred to as PoX in the literature) raises the fundamental question whether it is possible to utilize many of them in tandem and build multi-resource consensus protocols. The challenge in combining different resources is to achieve fungibility between them, in the sense that security would hold as long as the cumulative
adversarial power across all resources is bounded. 

In this work, we put forth Minotaur, a multi-resource blockchain consensus protocol that combines proof of work (PoW) and proofof-stake (PoS), and we prove it optimally fungible. At the core of our design, Minotaur operates in epochs while continuously sampling the active computational power to provide a fair exchange between the two resources, work and stake. Further, we demonstrate the ability of Minotaur to handle a higher degree of work fluctuation as compared to the Bitcoin blockchain; we also generalize Minotaur to any number of resources.

We demonstrate the simplicity of Minotaur via implementing a full stack client in Rust. We use the client to test the robustness of Minotaur to variable mining power and combined work/stake attacks and demonstrate concrete empirical evidence towards the suitability of Minotaur to serve as the consensus layer of a real-world blockchain.

## Build

To build the binary, run `cargo build --release`.

The first build could take several mintues, mostly due to building dependencies


<div align="center">
  <h1 align="center">Awesome ZKPs</h1>
  <p align="center">
    <a href="https://github.com/sindresorhus/awesome">
      <img alt="awesome list badge" src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg">
    </a>
    <a href="http://makeapullrequest.com">
      <img alt="pull requests welcome badge" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat">
    </a>
  </p>
  
  <p align="center">A curated list of awesome ZKP resources, libraries, tools and more.</p>
  <p align="center">Please check the <a href="CONTRIBUTING.md">contribution guidelines</a> for information on formatting and writing pull requests.</p>
  
</div>

### Contents

- [Introductions](#introductions)
- [Tutorials](#tutorials)
- [Programming Languages](#programming-languages)
- [Tools](#tools)
- [Books](#books)
- [Communities](#communities)
- [Other Curated Lists](#other-curated-lists)
- [Proof Systems](#proof-systems)
  - [zkSNARKs](#zksnarks)
  - [zkSTARKs](#zkstarks)
  - [Bulletproofs](#bulletproofs)
- [License](#license)

## Introductions
- [Understanding ZKPs Through Illustrated Examples](https://blog.goodaudience.com/understanding-zero-knowledge-proofs-through-simple-examples-df673f796d99)
- [Zero Knowledge Proofs: An Illustrated Primer by Matthew Green](https://blog.cryptographyengineering.com/2014/11/27/zero-knowledge-proofs-illustrated-primer/)
- [Zero Knowledge Proof and its Applications in Bitcoin](https://xiaohuiliu.medium.com/zero-knowledge-proof-and-its-applications-in-bitcoin-aca833d7d745)
- [zk-SNARKs on Bitcoin](https://xiaohuiliu.medium.com/zk-snarks-on-bitcoin-239d96d182bd)
- [ZKPs for Engineers: Introduction](https://blog.zkga.me/intro-to-zksnarks)


## Tutorials
- [zk Battleship interactive course by sCrypt](https://learn.scrypt.io/en/courses/630b1fe6c26857959e13e160)
- [Create Your First Zero-Knowledge Proof Program on Bitcoin](https://xiaohuiliu.medium.com/create-your-first-zero-knowledge-proof-program-on-bitcoin-ec159cc501f4): use ZoKrates
- [Intro to Circom and Snarkjs by Iden3](https://iden3-docs.readthedocs.io/en/latest/iden3_repos/circom/TUTORIAL.html)
- [Getting Started with zkSnarks on ZoKrates](https://blog.gnosis.pm/getting-started-with-zksnarks-zokrates-61e4f8e66bcc)
- [Proving Knowledge of a Hash Pre-Image with ZoKrates](https://blog.decentriq.com/proving-hash-pre-image-zksnarks-zokrates/)
- [Zokrates Hello World Walkthrough](https://hackmd.io/@adietrichs/HkH0OduZw)
- [Zero Knowledge Proofs Workshop - Zokrates Tutorial](http://extropy.foundation/workshops/zkp/zokrates.html)
- [A Practical Guide To Building Zero Knowledge dApps](https://kndrck.co/posts/practical_guide_build_zk_dapps/): Circom


## Programming Languages 
- [Introduction to Domain Specific Languages (DSLs)](https://youtu.be/kqnYbSmdcbA?t=392) by Alex Ozdemir
- [Programming Languages in ZKP](https://medium.com/delendum/thoughts-of-programming-languages-in-zkp-c906e96f056e) by Delendum Ventures: video is on [YouTube](https://www.youtube.com/channel/UCM7Dc3y3BVTTpprDidVV7iw)

| Name  | Type | GitHub | Documentation | 
| ------------- |:-------------:|:-------------:|:-------------:|
| ZoKrates     | Python subset   | https://github.com/Zokrates/ZoKrates | https://zokrates.github.io |
| Circom |  HDL   | https://github.com/iden3/circom | https://docs.circom.io |
| SnarkyJS | Typescript DSL | https://github.com/o1-labs/snarkyjs | https://docs.minaprotocol.com/en/zkapps/snarkyjs-reference | 
| Cairo     | for STARK  | https://github.com/starkware-libs/cairo-lang | https://cairo-lang.org/docs/ | 
| Leo      | Functional, statically-typed  | https://github.com/AleoHQ/leo | https://developer.aleo.org/developer/language/layout/ |


## Tools
- ZoKrates: a toolbox for zkSNARKs
  - [Bitcoin](https://github.com/sCrypt-Inc/zokrates)
  - [Ethereum](https://zokrates.github.io/)
- Snarkjs: zkSNARK implementation in JavaScript & WASM
  - [Bitcoin](https://github.com/sCrypt-Inc/snarkjs)
  - [Ethereum](https://github.com/iden3/snarkjs)


## Books

- [Proofs, Arguments, and Zero-Knowledge](https://people.cs.georgetown.edu/jthaler/ProofsArgsAndZK.pdf) (Justin Thaler, 2022)
- [A Graduate Course in Applied Cryptography](http://toc.cryptobook.us/book.pdf) (Dan Boneh and Victor Shoup, 2020)


## Communities
- [Zero-knowledge podcast](https://www.zeroknowledge.fm): #1 podcast for ZK
- [0xPARC: Applied ZK Learning Group](https://learn.0xparc.org/)
- [ZKProof](https://zkproof.org/): an academic and industry initiative for standardizing ZKPs


## Other Curated Lists
- [matter-labs: Awesome zero knowledge proofs](https://github.com/matter-labs/awesome-zero-knowledge-proofs)
- [ventali/awesome-zk](https://github.com/ventali/awesome-zk)
- [zkp.science](https://zkp.science)
- [Zero-Knowledge Proofs Starter Pack](https://ethresear.ch/t/zero-knowledge-proofs-starter-pack/4519)
- [gakonst/awesome-starknet](https://github.com/gakonst/awesome-starknet)


## Proof Systems
- [Comparison of the most popular zkp systems](https://github.com/matter-labs/awesome-zero-knowledge-proofs#comparison-of-the-most-popular-zkp-systems)

|                                       | SNARKs                     | STARKs                        | Bulletproofs    |
| ------------------------------------: | -------------------------: | ----------------------------: | --------------: |
| Algorithmic complexity: prover        | O(N * log(N))              | O(N * poly-log(N))            | O(N * log(N))   |
| Algorithmic complexity: verifier      | ~O(1)                      | O(poly-log(N))                | O(N)            |
| Communication complexity (proof size) | ~O(1)                      | O(poly-log(N))                | O(log(N))       |
| Trusted setup required?               | YES :unamused:             | NO :smile:                    | NO :smile:      |
- [zk-SNARKs vs. Zk-STARKs vs. BulletProofs](https://ethereum.stackexchange.com/questions/59145/zk-snarks-vs-zk-starks-vs-bulletproofs-updated) ![compare](./images/comparisons.png)
- [Comparing General Purpose zk-SNARKs](https://medium.com/coinmonks/comparing-general-purpose-zk-snarks-51ce124c60bd) ![compare snarks](./images/compare_snarks2.png)
- [Comparison of Different zk-SNARKs](https://zhuanlan.zhihu.com/p/40245832) ![compare snarks](./images/compare_snarks.jpeg)
- [A Cambrian Explosion of Crypto Proofs Eli Ben-Sasson](https://nakamoto.com/cambrian-explosion-of-crypto-proofs/)

### zkSNARKs

### zkSTARKs

### Bulletproofs

---

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, sCrypt Inc has waived all copyright and related or neighboring rights to this work.
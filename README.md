# Welcome to the Blockchain for Developers Decal (Fall 2026)!

This decal is designed to provide students with a comprehensive overview of relevant topics in blockchain development, as well as hands-on experience in developing and deploying their own smart contracts & sovereign Cosmos blockchains.

Blockchain is currently one of the fastest-growing industries in the technology sector. In response to this shortage of blockchain developers, this course aims to teach students the technical fundamentals of blockchains, the Solidity programming language, the Cosmos ecosystem, as well as industry-relevant tools such as Metamask, Wagmi, Foundry, Rust, and Cosmos SDK such that students will be equipped with industry-relevant experience in an accessible, collaborative environment. We hope that through this course, students will become more confident in their ability to develop and deploy blockchain-based solutions on important industry issues.

## Getting the Homework

Clone this repo with its submodules (HW3 and HW5 use Foundry libraries pulled in as git submodules):

```
git clone --recurse-submodules https://github.com/BerkeleyBlockchain/fa26-dev-decal.git
```

If you already cloned without `--recurse-submodules`, run `git submodule update --init --recursive` from the repo root.

## Homework

Lessons are on Mondays. Each homework is due at **11:59 PM PT** on the day of the next lesson.

| Homework | Folder | Submission Form | Due (11:59 PM PT) |
| --- | --- | --- | --- |
| HW1: Build a Blockchain in Python | [HW1 - Build a Blockchain in Python](HW1%20-%20Build%20a%20Blockchain%20in%20Python) | [HW1 form](https://docs.google.com/forms/d/1AtLCSsmPeCQVa5ig0tnJFjhOwRgP3s3561cc2YlNkY4/viewform) | Mon Sep 28, 2026 |
| HW2: Deploy Your ERC721 | [HW2 - Deploy Your ERC721](HW2%20-%20Deploy%20Your%20ERC721) | [HW2 form](https://docs.google.com/forms/d/1lePpyJxGkmJsJhlT_uVZwop67u85_57GT7A9vwlzo48/viewform) | Mon Oct 12, 2026 |
| HW3: Implementing NFT Marketplace | [HW3 - Implementing NFT Marketplace](HW3%20-%20Implementing%20NFT%20Marketplace) | [HW3 form](https://docs.google.com/forms/d/1NIWhh8DriL0cb3qgozOepOkfydOc8Lp8QlCOsG3rQHw/viewform) | Mon Oct 19, 2026 |
| HW4: Ethers.js | [HW4 - Etherjs](HW4%20-%20Etherjs) | [HW4 form](https://docs.google.com/forms/d/11aZrIp4cOSUDAmmcTzDHMbdd2rvfGhnkye1pX21qI8c/viewform) | TBD (the next lesson after Oct 19) |
| HW5: Gas Optimization | [HW5 - Gas Optimization](HW5%20-%20Gas%20Optimization) | [HW5 form](https://docs.google.com/forms/d/1LFpOjEEskxrguGSdc6SF7p5JrYx-WtphJzflrAgsS7k/viewform) | TBD |
| HW6: Rust Basics | [HW6 - Rust Basics](HW6%20-%20Rust%20Basics) | [HW6 form](https://docs.google.com/forms/d/1a8WFbdVmpUqkYKfWYAQjVv0Xlx17GoNRvwevvHH-2ig/viewform) | TBD |
| HW7: CosmWasm | [HW7 - COSMWASM](HW7%20-%20COSMWASM) | [HW7 form](https://docs.google.com/forms/d/1i_amTzIdpPNik3woKq7XUolO1mTPkDyvmFMaogwKmb0/viewform) | TBD |

## Contact Info

For help/questions, email: dev-decal@blockchain.berkeley.edu

### Course Instructors
- Yadukrishna Ragu
- Anthony Kobzar
- Nithya Appannagaari

## Weekly Lecture Topics/YouTube Videos
### Week 1
But How Does BitCoin Actually Work: https://www.youtube.com/watch?v=bBC-nXj3Ng4 - Great video on Bitcoin's underlying structure. Worth the watch.

Blockchain 101 - A Visual Demo: https://www.youtube.com/watch?v=_160oMzblY8 - Good video for understanding how nonce values are found for Bitcoin block headers + how blocks link together to form a "block-chain".

### Week 2
#### Topic Preview

##### Development & Ecosystem Tools
- **MetaMask**: Crypto wallet for Ethereum and any other EVM-compatible chain.

- **Etherscan**: Block explorer for Ethereum. View and verify transactions, addresses, smart contracts, tokens, and blocks on Ethereum.

- **Foundry**: Development framework for Ethereum smart contracts. Helps developers write, test, deploy, and interact with contracts.

- **Remix IDE**: Online IDE for writing, testing, and deploying Ethereum smart contracts. No installation needed!

##### Networks & Infrastructure
- **Testnets (Test Networks)**: Versions of Ethereum that behave like the real chain but use valueless test ETH. They let developers deploy, test, and debug smart contracts or dApps without risking real money.

- **RPC (Remote Procedure Call)**: The “bridge” (URL endpoint) your wallet/dApp uses to connect to a blockchain network (mainnet, testnet, or another chain).

##### Learning Solidity
- **Solidity**: A headstart on the Solidity programming language. *CryptoZombies* is an interactive game that teaches you how to write Solidity smart contracts by making your own zombie NFT! Great way to get familiar with Solidity. 🙂

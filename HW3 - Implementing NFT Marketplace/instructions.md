
# Homework 3 - Building an NFT Marketplace

**Due:** Mon Oct 19, 2026, 11:59 PM PT

In this homework, you will expand on the NFT contract you built in HW2 to build an NFT Marketplace contract.

Created by Siddhant Satapathy and Daniel Gushchyan

## Getting Started

### Cloning Github Repository

This homework lives in the Fall 2026 course repo: https://github.com/BerkeleyBlockchain/fa26-dev-decal/tree/main/HW3%20-%20Implementing%20NFT%20Marketplace. If you already cloned that repo, use the `HW3 - Implementing NFT Marketplace` directory. 

You will be editing the src/NFTMarketplace.sol contract.

### Foundry setup

From the previous HW, you should have Foundry set up. For this homework, we use external [OpenZeppelin contracts](https://www.openzeppelin.com/contracts) with Forge. 

OpenZeppelin is a repository of common ERC20 and ERC721 smart contracts that have been thoroughly tested and verified, and are used by most dApps. We will be inheriting from these contracts and building on top of them.

`forge-std` (v1.4.0) and `openzeppelin-contracts` (v4.8.1) are already included in `lib/` as git submodules, and `remappings.txt` already points at them. To set them up:

1. From the <b>root of the fa26-dev-decal repo</b>, run:
```
git submodule update --init --recursive
```
(Skip this if you cloned with `--recurse-submodules`.) If you downloaded only this folder instead of cloning the repo, run `forge install --no-git foundry-rs/forge-std@v1.4.0 OpenZeppelin/openzeppelin-contracts@v4.8.1` in the `HW3 - Implementing NFT Marketplace` directory instead (leave out `--no-git` if that folder is inside your own git repo). Use OpenZeppelin v4.8.1: newer versions removed `Counters.sol`, which this homework imports.
2. In the `HW3 - Implementing NFT Marketplace` directory, run
```
forge build
```

At this stage, we haven't filled out the NFTMarketplace.sol contract yet. Thus, the compilation will fail.

### Looking at the NFT Marketplace Contract (demo)

### Filling in the remaining functions

Now fill in updateListingPrice(), getListingPrice(), fetchItemsListed(), fetchMyNFTs(), and fetchMarketItems() functions. 

After you have filled these in, run 
```
forge test -vv
```
to verify that these functions work properly. Our tests are not comprehensive, but they test the basic functionality of these functions. 

You can specify the verbosity of the output by changing the number of v's. ``` forge test ``` is the not verbose, while ``` forge test -vvvv ``` is extremely verbose.



## Submission

**Due:** Mon Oct 19, 2026, 11:59 PM PT

Submit your NFTMarketplace.sol file and a screenshot of your 4/4 passed tests on this form:

https://docs.google.com/forms/d/1NIWhh8DriL0cb3qgozOepOkfydOc8Lp8QlCOsG3rQHw/viewform

Congratulations! You've now deployed an operational NFT marketplace! 

Please email us if you have any issues!

### Troubleshooting

- If you have issues with forge build not recognizing solidity v0.8.19, then add this line to foundry.toml to anchor the solidity version to v0.8.13. 

```
solc_version = "0.8.13"
```
If this doesn't work, then reinstall Solidity and try this step again.

- If the OpenZeppelin imports are not recognized, ensure that these lines are in remappings.txt. If not, then add them. Additionally, if you are using VSCode, then please go into settings and search for Solidity. Ensure that Package Default Dependencies Contracts Directory is set to src and Package Default Dependencies Directory is set to lib.

```
openzeppelin-contracts/=lib/openzeppelin-contracts/
@openzeppelin/=lib/openzeppelin-contracts/
```

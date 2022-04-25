# MerkleTreeAuth

## Step 00 - Introduction

## Step 01 - Merkle Tree

In order to create a __Merkle Proof Authentification__, you are going to need to create a new solidity contract called __MerkleTreeAuth__. This contract aims to store the merkle tree leafs and check if a element is included inside this tree:

- The first step is to create the root of the tree, to do this you are going to create a __constructor__ which will set this root

- And now, you are going to create a __isAuthorized__ function which take as parameter a __bytes32[]__ which is the merkleProof we need to check. It has a visibility of __public view__ and it must return a __boolean__ that will determine if the element is inside the tree or not.

In the next step, you are going to create tests for the contract in ts using mocha

### Documentation

To do this, you should use the __0.8.0__ solidity version.

We are going to use one of the openzepplin contracts called MerkleProof.sol to help us in this task
```ts
import "@openzeppelin/contracts/utils/cryptography/MerkleProof.sol";
```

https://docs.soliditylang.org/en/v0.8.0/

https://docs.soliditylang.org/en/v0.8.0/introduction-to-smart-contracts.html#a-simple-smart-contract

https://docs.openzeppelin.com/contracts/3.x/api/cryptography

## Step 02 - Merkle Tree

### Documentation

## Step 03 - Deploy Contract

In this step we will deploy our MerkleTreeAuth Contract.</br>
To do this we will create a main function.</br>
In it, we will need to define three things.</br>

- Collection of all signers on ethers.
- Creating our leafsNodes which simply returns a keccak256 of the account addresses.
- Create our merkleTree which takes as parameters our leafNode and a MerkleRoot.

All you have to do is to get your **MerkleTreeAuth** contract and deploy it !

Don't hesitate to use console.log to display the address of your MerkleProof in order to check the data.

### Documentation

You may need all three of these imports:
```ts
import { keccak256 } from "ethers/lib/utils";
import { ethers } from "hardhat";
import { MerkleTree } from "merkletreejs";
```

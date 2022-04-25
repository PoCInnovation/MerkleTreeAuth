# MerkleTreeAuth

## Step 00 - Introduction

## Step 01 - Merkle Tree

In order to create a __Merkle Proof Authentification__, you are going to need to create a new solidity contract called __MerkleTreeAuth__. This contract aims to store the merkle tree leafs and check if a element is included inside this tree:

- The first step is to create the root of the tree, to do this you are going to create a __constructor__ which will set this root

- And now, you are going to create a __isAuthorized__ function which take as parameter a __bytes32[]__ which is the merkleProof we need to check. It has a visibility of __public view__ and it must return a __boolean__ that will determine if the element is inside the tree or not.

In the next step, you are going to see how to see how to create the merkle tree root using hardhat and merkletree.

### Documentation

To do this, you should use the __0.8.0__ solidity version.

We are going to use one of the openzepplin contracts called MerkleProof.sol to help us in this task
```
import "@openzeppelin/contracts/utils/cryptography/MerkleProof.sol";
```

## Step 02 - Merkle Tree

### Documentation

## Step 03 - Deploy

### Documentation

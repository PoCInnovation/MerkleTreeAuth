# MerkleTreeAuth

## Step 00 - Introduction

### Documentation

## Step 01 - Merkle Tree

In order to create a merkle proof authentification, you are going to need to create a new solidity contract called MerkleTreeAuth. This contract aims to store the merkle tree leafs and check if a element is included inside this tree.

The first step is to create the root of the tree, to do this you are going to create a constructor which will set this root

And now, you are going to create a isAuthorized function which has visibility as public view that will return a boolean saying if the element is inside the tree or not.

In the next step, you are going to see how to see how to create the merkle tree root using ts.

### Documentation

To do this, you should use the 0.8.0 version of solidity.

To help us in this task, we're going to use one of the openzepplin contracts called MerkleProof.sol

## Step 02 - Merkle Tree

### Documentation

## Step 03 - Deploy

### Documentation

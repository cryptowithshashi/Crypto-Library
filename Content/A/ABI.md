<!--
title: "Application Binary Interface (ABI)"
slug: "abi"
short: "Resources for understanding and using the ABI with EVM smart contracts."
difficulty: "Beginner → Advanced"
tags: ["solidity","ethereum","abi","dev-tools"]
canonical: "https://docs.soliditylang.org/en/latest/abi-spec.html"
last_reviewed: "2025-08-24"
reviewer: "TBD"
-->

# Application Binary Interface

This page collects authoritative explainers, tutorials, videos, and tools for understanding and using the Application Binary Interface (ABI) with EVM smart contracts. We do not define every term here, instead we link to clear, practical resources and include a one-line note for each item so you can pick the right resource for your level and use-case.

## Why it matters

- ABIs map contract functions & types to the byte-level encoding used by the EVM necessary to call contracts programmatically.

- Correct ABI handling prevents bugs, security issues, and decoding errors when reading events or calling functions.

- Understanding ABI is required for: building frontends/backends that talk to contracts, decoding transaction calldata and event logs, writing tools (fuzzers, analyzers), and safely composing low-level transactions.

## Most practical resources (developer-focused)

- Contract ABI Specification (Solidity Lang): canonical source for encoding rules; must-read for debugging low-level issues.

- Interacting with Contracts (Ethers.js): the practical guide for the most-used JavaScript library; shows how to apply ABIs in apps.

- Application Binary Interface (Ethereum.org): friendly conceptual overview from the foundation; good on-ramp.

- abi-decoder (ConsenSys): practical JS library for decoding logs & calldata quickly.

- "What Are ABI and Bytecode in Solidity?" (Chainlink blog): Remix walkthrough that bridges theory → practice.

- fetch_contract_abi (DEV.to / MannyUncharted): simple script for fetching ABIs programmatically (real-world utility).


## Docs

| Title | Source | Why include | Difficulty |
| :--- | :--- | :--- | :--- |
| [Contract ABI Specification](https://docs.soliditylang.org/en/latest/abi-spec.html) | Solidity Lang | The official, canonical specification of ABI structure & encoding rules. | Advanced |
| [Interacting with Contracts (Ethers.js)](https://docs.ethers.org/v5/api/contract/contract/) | Ethers.js docs | How the Interface / Contract helpers use ABIs in JS; essential for frontends/backends. | Intermediate |
| [Contract Instances](https://docs.web3js.org/api/web3-eth-contract/class/Contract/)| Web3.js docs | Documentation for working with ABIs in web3.js, good for legacy projects. | Intermediate |
| [Interacting with your contracts](https://hardhat.org/hardhat-network/docs) | Hardhat docs | Shows how to get ABIs during compilation & how to use them in dev workflow. | Intermediate |
| [Interacting with Contracts](https://viem.sh/docs/getting-started) | Viem | Typesafe/modern usage patterns for ABIs and contract calls. | Intermediate |
| [Application Binary Interface](https://docs.web3j.io/4.14.0/smart_contracts/application_binary_interface/) | Ether.js docs | Java implementations of all ABI types | Intermediate |


## Articles

| Title | Author / Source | Why include | Difficulty |
| :--- | :--- | :--- | :--- |
| [What is the Solidity ABI?](https://www.alchemy.com/overviews/solidity-abi) | Alchemy | Bridges gap between theory and practice with code snippets (ethers.js). | Beginner |
| [What Are ABI and Bytecode in Solidity?](https://blog.chain.link/what-are-abi-and-bytecode-in-solidity/) | Chainlink Blog | Step-by-step Remix walkthrough on ABI vs bytecode. | Beginner–Intermediate |
| [Solidity Tutorial: all about ABI](https://coinsbench.com/solidity-tutorial-all-about-abi-46da8b517e7) | CoinsBench | Explains JSON ABI, selectors and encoding pitfalls. | Intermediate |
| [A Developer Guide to Smart Contract ABI](https://blockchain.oodles.io/dev-blog/smart_contract_abi/) | Oodles Blockchain | Walks through ABI internals and JSON structure. | Intermediate |
| [ABI-encode and decode using Solidity](https://medium.com/coinmonks/abi-encode-and-decode-using-solidity-2d372a03e110) | João Paulo Morais / Medium | Practical Solidity examples of abi.encode / abi.decode. | Intermediate |
| [The Anatomy of an ABI-Encoded Function Call](https://learnevm.com/chapters/abi-encoding/anatomy) | LearnEVM.com | Annotated walk-through of actual calldata bytes. | Advanced |
| [ABI and Bytecode Explained](https://chainstack.com/essential-web3-calls/) | Chainstack | Explains how bytecode and ABI relate — useful for deploy/decode tasks. | Beginner |


## Youtube


- [Solidity ABI Encode | How To Encode ABI In Solidity Smart Contract | Solidity Course 2022](https://www.youtube.com/watch?v=Br5spvcKpXw) - This video provides a tutorial on ABI encoding in Solidity smart contracts, explaining how it's used to generate and retrieve data. by Daulat Hussain

- [What is ABI in SOLIDITY (and BYTECODE)? Ethereum Developer Mental Models for Web3 Developers.](https://www.youtube.com/watch?v=Z7UNjk_roXI) - This video provides an in-depth explanation of bytecode and ABI (Application Binary Interface) within the context of the Ethereum world. by Zubin Pratap

- [What is an ABI?](https://www.youtube.com/watch?v=xamI-lHOufM) - A comprehensive guide to understanding what an ABI (Application Binary Interface) is, differentiating it from an API, detailing its elements, and demonstrating two ways to generate it for a smart contract. by QuickNode

- [EVM Bytecode ABI Gas and Gas Price](https://www.youtube.com/watch?v=HcOWNxL3Iy0) - An introduction to fundamental concepts and terminology in smart contract programming. by Smart Contract Programmer

- [4.3 ABI - the menu of a smart contract](https://www.google.com/search?q=https://www.youtube.com/watch%3Fv%3DaMQCrWWW83o) - This video explains what an Application Binary Interface (ABI) is in the context of smart contracts, comparing it to an Application Programming Interface (API) in the traditional web. by Surge Women

- [Solidity Programming | What is an ABI in solidity?](https://www.youtube.com/watch?v=92cnCI9pxAQ) - An overview of ABI (Application Binary Interface) and bytecode in the context of smart contract development. by Dro Orozco

- [Week 2 - International School Algorand Smart Contracts: Writing ABI Compliant Smart Contracts PyTEAL](https://www.youtube.com/watch?v=USLcyfVD_ws) - This video provides an in-depth explanation of the Algorand Application Binary Interface (ABI) and how to write ABI-compliant smart contracts using PyTEAL. by Algorand Foundation

- [Ethereum contract Application Binary Interface](https://www.youtube.com/watch?v=F_l4HycnHAI) - This video explains what an Application Binary Interface (ABI) is and its purpose in the context of Ethereum smart contracts. by Mobilefish.com

- [Solidity ABI & ByteCode - Part 3 | Complete Course](https://www.youtube.com/watch?v=AKrWU_fF2vI) - This video, part three of the Solidity programming language course, explains the process of contract compilation, focusing on what ABI and bytecode are. by ETechViral

- [How to import a Solidity / smart contract ABI into a Dapp Frontend? 4 solutions (including webpack)](https://www.youtube.com/watch?v=DfxW3QcK8Hs) - An introduction to the Application Binary Interface (ABI) of a smart contract and demonstrates four different methods for importing it into the frontend of a DApp. by EatTheBlocks

- [5 PyTeal Tutorial for Beginners | ABI Types - More Data Types on Algorand Smart Contract](https://www.youtube.com/watch?v=6mM4_137CqA) - This video introduces ABI (Application Binary Interface) types with ARC-4, which provides support for a wider variety of data types in Algorand smart contracts, making them more intuitive to code. by Algorand Developers

- [Open Build - Frontend setup and using the Etherscan ABI API](https://www.youtube.com/watch?v=AwM7alAEsng) - This video is an open build session focusing on the initial frontend development and integration with the Etherscan API for a web3 event router application. by Long Island Blockchain

- [Mastering ABI Encoding for Solidity and Ethereum (Full Examples Included)](https://www.youtube.com/watch?v=upVloLUw5Z0) - An in-depth explanation of ABI (Application Binary Interface) encoding and decoding, which is crucial for understanding how smart contracts communicate on Ethereum and Solidity. by Jesper Kristensen (jtk.eth)

- [Get a Solidity contract ABI programmatically with JavaScript & Etherscan API | Stop hardcoding ABIs](https://www.youtube.com/watch?v=dArGajlpng0) - This video demonstrates how to programmatically retrieve a contract's Application Binary Interface (ABI) using the Etherscan API and then interact with that contract using Ethers.js. by Blockman Codes

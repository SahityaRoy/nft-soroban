The provided Rust codebase comprises a set of smart contracts designed for managing Non-Fungible Tokens (NFTs) within the Soroban environment. Here's a summary of the README.md file:

### Overview
- The project contains a `src` folder and a `Cargo.toml` file.
- Within `src`, there are various Rust smart contracts imported into `contract.rs`.
- These contracts are structured to allow for inheritance of functionality, inspired by existing fungible token contracts in Soroban.

### Contracts
1. **admin.rs**: Manages system administrators, enabling checks, reads, writes, and authentication verification.
2. **approval.rs**: Handles approvals for specific actions, including reading, writing, and checking approval status.
3. **balance.rs**: Manages token balances, supply, minted status, and related functions such as reading, writing, and incrementing balances.
4. **contract.rs**: The main function responsible for NFT operations, including minting and transfers, adhering to the ERC721 standard.
5. **event.rs**: Publishes events for various actions such as transfers, setting administrators, minting, burning, and approvals.
6. **interface.rs**: Contains interfaces for contract functions.
7. **lib.rs**: Modular implementation for NFT system designed for Soroban environments.
8. **metadata.rs**: Handles token metadata operations like reading and writing token names, symbols, and URIs.
9. **owner.rs**: Manages token ownership, providing functions for reading, writing, and checking owners.
10. **storage_types.rs**: Defines contract types for managing approvals and data keys in the system.

### Steps to Compile
1. Set up Soroban CLI as per the provided documentation.
2. Run `soroban contract build` after installation.
3. Upon successful compilation, a `target` folder will be created containing the wasm executable.

Overall, the README provides an overview of the contract structure, functionalities, and instructions for compiling the code using Soroban CLI.

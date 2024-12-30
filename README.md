# Character Upgrade Smart Contract

This smart contract is designed for the MultiversX blockchain. It allows users to upgrade a character's defense attribute using a tool NFT. The character and tool are both represented as NFTs, and the upgrade process consumes the tool NFT.

## Features

- **Character Management**: Store and manage character attributes such as defense.
- **NFT Integration**: Use NFTs for character and tool representation.
- **Attribute Upgrades**: Increment a character's defense by consuming a tool NFT.

## Prerequisites

- [Rust](https://www.rust-lang.org/) and [Cargo](https://doc.rust-lang.org/cargo/) installed.
- MultiversX CLI tools for deploying and interacting with smart contracts.

## Project Structure


character_upgrade_contract/
├── Cargo.toml
└── src
└── lib.rs

Copy

## Setup and Deployment

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd character_upgrade_contract
Build the Contract: Compile the smart contract to WebAssembly.

cargo build --release --target=wasm32-unknown-unknown
Deploy the Contract: Use MultiversX tools to deploy the compiled Wasm file to the MultiversX Devnet or Mainnet.

Interact with the Contract: Use the MultiversX Devnet Explorer or CLI to call endpoints such as upgradeCharacter.

Contract Usage
Upgrade Character
Endpoint: upgradeCharacter
Parameters:
character_nft_id: The ID of the character NFT.
character_nonce: The nonce of the character NFT.
tool_nft_id: The ID of the tool NFT.
tool_nonce: The nonce of the tool NFT.
View Character
Endpoint: getCharacter
Parameters:
character_nft_id: The ID of the character NFT.
character_nonce: The nonce of the character NFT.
Verification
Code Verification: Review the contract code in src/lib.rs.
ABI Verification: Check the contract's ABI for endpoint definitions and parameter types.
# FUTTURE_BC_597
Emmanuel Basakeng Blockchain and Crypto internship Future Interns
# QuickToken (QTK)

This project demonstrates a simple implementation of an **ERC-20 token** using **Solidity**, **OpenZeppelin**, and **Remix IDE**. It was deployed and tested on the **Remix VM (Prague)** environment.

## 🚀 Token Details

- **Token Name**: QuickToken  
- **Symbol**: QTK  
- **Total Supply**: 1000 QTK (1000 * 10^18 units)  
- **Standard**: ERC-20  
- **Decimals**: 18  
- **Deployer Address**: `0x5B38Da6a701c568545dCfcB03FcB875f56beddC4`  
- **Contract Address (Simulated)**: `0xd8b934580fcE35a11B58C6D73aDeE468a2833fa8`  

## 📜 Smart Contract Code

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract MyToken is ERC20 {
    constructor(uint256 initialSupply) ERC20("QuickToken", "QTK") {
        _mint(msg.sender, initialSupply * 10 ** decimals());
    }
}

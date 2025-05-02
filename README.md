README.md# SPACEDOGE ($SPDG)

SPACEDOGE is a decentralized Ethereum-based meme token with a mission to build trust through transparency, zero dev control, and real community power. No tricks. No rug. Just rocket fuel.


## 💡 Key Features

- ✅ Ownership Renounced  
- 🔥 460 Billion Tokens Burned  
- 💧 500 Billion Tokens Supplied to Uniswap V2  
- 🪂 20 Billion Airdropped to Community  
- ➕ 20 Billion Additional Sent to Uniswap V2  
- ❌ No Mint, No Blacklist, No Dev Wallet  
- 🔒 Contract Audit In Progress (SolidityScan)


## 🔗 Official Links

- 🌐 Website: [https://spacedoges.xyz](https://spacedoges.xyz)  
- 🐦 Twitter: [@SpaceDogeETH](https://twitter.com/SpaceDogeETH)  
- 📣 Telegram: [https://t.me/+546CC3Nn7Eo4MzRh](https://t.me/+546CC3Nn7Eo4MzRh)

---

## 🔐 Smart Contract Info

- **Token Symbol:** SPDG  
- **Blockchain:** Ethereum (ERC-20)  
- **Contract Address:** *(Insert Here)*


## 👑 Powered by the Community. Led by SH.
# SPACEDOGE ($SPDG)

SPACEDOGE is a decentralized Ethereum-based meme token with a mission to build trust through transparency, zero dev control, and real community power. No tricks. No rug. Just rocket fuel.


// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

contract SpaceDoge is ERC20, Ownable {
    constructor() ERC20("SPACEDOGE", "SPDG") {
        _mint(msg.sender, 1_000_000_000_000 * 10 ** decimals());
        renounceOwnership(); // Ownership renounced on deployment
    }
}








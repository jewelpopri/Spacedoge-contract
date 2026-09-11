token Contract Address:0xf46CCb9E08fB7e32eED560C87d5e583a59A43420

**Contract Address:**  
`0xYourTokenContractAddressHere`  
[View on Etherscan](https://etherscan.io/token/0xYourTokenContractAddressHere)

**Burn Proof Transactions:**  
burn#1 https://etherscan.io/tx/0xf65fd2566e9eebf2bff5f9404ef38fdf5465fb9c354543150b91aa3e0815766c      (460,000,000,000 SPDG · Apr 30, 2025)
burn#2 https://etherscan.io/tx/0x2d2ddee3f14fd46eb6fdaa8f9073adb6aa0787470d747347dde9d79906b12daf      (480,000,000,000 SPDG · May 04, 2025)
burn#3 https://etherscan.io/tx/0x91cd036aa1370dacd299c01e42a60805314d01078a8c7c05e5ca596005e8bd39      (103,000,000 SPDG · Verified)
burn#4 https://etherscan.io/tx/0xee93f834f7d6a58c8966f88cbcaf6ca4397a024c2661ee05dd753d8edcc55c06      (94,541,953 SPDG · Verified)
burn#5 https://etherscan.io/tx/0x83f854a290df0dcca664de55a02f868928c698ec06cd14f0bba2a936d30efbd7      (500,000,000 SPDG · Verified)
burn#6 https://etherscan.io/tx/0x1e0167f97219d1698ab2399b6b086dda5ecfe4a9175c6bc0d9273ac97c3f0264      (10,000,000,000 SPDG · Verified)
Official SPDG Burn Vault Address:
All burn transactions route to the verified burn vault. Permanently holding burned tokens — zero probability of recovery.
0xD89fa6A040f04367f5115Dd767db1BDA83B02057
https://etherscan.io/address/0xD89fa6A040f04367f5115Dd767db1BDA83B02057
       
**Tokenomics Summary**

- Initial Supply: 1,000,000,000,000 SPDG
- Current Burned Supply: See publicly verifiable on-chain burn transactions
- Current Circulating Supply: See current on-chain supply data
- No additional minting
- No developer wallet

Website: https://spacedoges.com
X: https://x.com/spacedogexyz
Telegram: https://t.me/joinspacedoge

/**
 *Submitted for verification at Etherscan.io on 2025-04-29
*/

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SpaceDoge {
    string public name = "SPACEDOGE";
    string public symbol = "SPDG";
    uint8 public decimals = 18;
    uint256 public totalSupply;

    mapping(address => uint256) public balanceOf;
    mapping(address => mapping(address => uint256)) public allowance;

    event Transfer(address indexed from, address indexed to, uint256 value);
    event Approval(address indexed owner, address indexed spender, uint256 value);

    constructor() {
        totalSupply = 1_000_000_000_000 * (10 ** uint256(decimals)); // 1 Trillion SPDG
        balanceOf[msg.sender] = totalSupply;
        emit Transfer(address(0), msg.sender, totalSupply);
    }

    function transfer(address to, uint256 value) public returns (bool success) {
        require(balanceOf[msg.sender] >= value, "Insufficient balance");
        balanceOf[msg.sender] -= value;
        balanceOf[to] += value;
        emit Transfer(msg.sender, to, value);
        return true;
    }

    function approve(address spender, uint256 value) public returns (bool success) {
        allowance[msg.sender][spender] = value;
        emit Approval(msg.sender, spender, value);
        return true;
    }

    function transferFrom(address from, address to, uint256 value) public returns (bool success) {
        require(balanceOf[from] >= value, "Insufficient balance");
        require(allowance[from][msg.sender] >= value, "Allowance exceeded");
        balanceOf[from] -= value;
        balanceOf[to] += value;
        allowance[from][msg.sender] -= value;
        emit Transfer(from, to, value);
        return true;
    }
}





**SPACEDOGE (\$SPDG) WHITEPAPER**

---

🚀 **SPACEDOGE: The Future of Space-Themed Community Tokens**

---

**1. Introduction**
SPACEDOGE (\$SPDG) is a next-generation decentralized meme token launched on the Ethereum blockchain. Inspired by the limitless possibilities of space exploration and the global Doge phenomenon, SPACEDOGE aims to build a strong, honest, and fully decentralized community-driven project with no developer wallets, no taxes, and no centralized control.

---
**2. The Problem
Many community tokens rely heavily on short-term attention and complex token structures. SPACEDOGE was created with a simpler approach focused on transparent on-chain activity, straightforward token mechanics, and community participation.

---

**3. The Solution: SPACEDOGE**
SPACEDOGE provides a true community-first solution:

* ✅ 0% Buy Tax / 0% Sell Tax
* ✅ No Developer Wallets
* ✅ Ownership Renounced
* ✅ Powered entirely by community strength and transparency

---

**4. Tokenomics**

| Metric             | Value             |
| ------------------ | ----------------- |
| Name               | SPACEDOGE         |
| Symbol             | SPDG              |
| Blockchain         | Ethereum (ERC-20) |
| Decimals           | 18                |
| Total Supply       | 1 Trillion SPDG   |
| Circulating Supply | See current on-chain supply data | 
| Buy/Sell Tax       | 0%                |
| Liquidity Status   |Original Uniswap V2 LP locked until 2030 |
| Developer Wallets  | None              |

---
**5 🛡️ Security & Transparency**

* 0% transaction tax
* Contract ownership renounced
* No additional token minting
* Token burns publicly verifiable on Ethereum
* Contract source code publicly available and verified
* On-chain activity independently verifiable


* └── 🔒 20B LP (Uniswap V2) – Locked until 2030
* └── 🎁 20B Community & Operations — Community rewards, marketing & project operations|
* └── ♻️ 20B Migration – For old SPDG holders

✅ 100% accounted for — zero hidden tokens

---

**🛡️ Security & Trust**


* 🔐 All LP tokens from 20B locked until 2030
* 🧾 No dev wallet, no taxes, no presale
* 🔍 Contract verified + audited
* 🪪 Ownership renounced
* ✅ Etherscan verified
* 🧑‍🚀 Community-owned forever

---

## 6. Roadmap

| Phase | Milestones |
|------|------------|
| Phase 1 | SPDG Token Launch on Ethereum and Initial Uniswap V2 Liquidity |
| Phase 2 | Community Development and On-Chain Token Burns |
| Phase 3 | Website Development and Project Documentation |
| Phase 4 | CoinGecko and CoinMarketCap Applications |
| Phase 5 | Community Growth, Strategic Partnerships and Ecosystem Development |
| Ongoing | Liquidity Development, Community Initiatives and Project Transparency |

**7. Community Power**
SPACEDOGE belongs to its community. Every holder is a co-pilot in the journey through the crypto galaxy. The mission is clear: Build, Promote, and Grow \$SPDG organically through strong community bonds.

* Social media marketing
* Viral campaigns
* Strategic partnerships

---

**8. Legal Disclaimer**
This document is for informational purposes only. It does not constitute financial, legal, or investment advice. Cryptocurrencies are highly volatile and involve significant risks. Always DYOR (Do Your Own Research).

---

💪 **SPACEDOGE: TO THE MOON AND BEYOND 🚀**

* **Website:** [https://spacedoges.com](https://spacedoges.com)
* **Twitter:** [https://twitter.com/spacedogexyz](https://twitter.com/spacedogexyz)
* **Telegram:** [https://t.me/joinspacedoge](https://t.me/joinspacedoge)
* **GitHub:** [https://github.com/jewelpopri](https://github.com/jewelpopri)

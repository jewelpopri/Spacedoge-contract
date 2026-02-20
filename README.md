token Contract Address:0xf46CCb9E08fB7e32eED560C87d5e583a59A43420

**Contract Address:**  
`0xYourTokenContractAddressHere`  
[View on Etherscan](https://etherscan.io/token/0xYourTokenContractAddressHere)

**Burn Proof Transactions:**  
- [Burn TX #1](https://etherscan.io/tx/0x2d2ddee3f14fd46eb6fdaa8f9073adb6aa0787470d747347dde9d79906b12daf)  
- [Burn TX #2](https://etherscan.io/tx/0xf65fd2566e9eebf2bff5f9404ef38fdf5465fb9c354543150b91aa3e0815766c)

**Tokenomics Summary:**  
- Total Supply: 1,000,000,000,000 SPDG  
- Total Burned: 940,000,000,000 SPDG  
- Circulating Supply: 60,000,000,000 SPDG  
- No dev wallets, no taxes, ownership renounced

**Website:** [https://spacedoges.xyz](https://spacedoges.xyz)  
**Whitepaper:** [Link to Whitepaper]  
**Community:** [Telegram](https://t.me/spacedogexyz), [Twitter](https://twitter.com/spacedogexyz)

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

**2. The Problem**
Cryptocurrency investors today face countless projects with hidden developer fees, fake liquidity, and centralized control. Many projects prioritize profit over community, leading to frequent rugpulls and trust issues.

---

**3. The Solution: SPACEDOGE**
SPACEDOGE provides a true community-first solution:

* ✅ 0% Buy Tax / 0% Sell Tax
* ✅ 100% Liquidity Added and Burned Forever
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
| Circulating Supply | 60 Billion SPDG   |
| Buy/Sell Tax       | 0%                |
| Liquidity Status   | Burned Forever    |
| Developer Wallets  | None              |

---

**5. Final SPACEDOGE (SPDG) Token Distribution**

| Category         | Amount                 |
| ---------------- | ---------------------- |
| Total Supply     | 1,000,000,000,000 SPDG |
| 1st Burn (TX 1)  | 460,000,000,000 SPDG   |
| 2nd Burn (TX 2)  | 480,000,000,000 SPDG   |
| 🔥 Total Burned  | 940,000,000,000 SPDG   |
| Remaining Supply | 60,000,000,000 SPDG    |

* └── 🔒 20B LP (Uniswap V2) – Locked until 2030
* └── 🎁 20B Airdrop Reserve – For community distribution
* └── ♻️ 20B Migration – For old SPDG holders

✅ 100% accounted for — zero hidden tokens

---

**🛡️ Security & Trust**

* 🔥 94% of total supply burned
* 🔐 All LP tokens from 20B locked until 2030
* 🧾 No dev wallet, no taxes, no presale
* 🔍 Contract verified + audited
* 🪪 Ownership renounced
* ✅ Etherscan verified
* 🧑‍🚀 Community-owned forever

---

**6. Roadmap**

| Phase     | Milestones                                             |
| --------- | ------------------------------------------------------ |
| Phase 1   | Token Launch, Liquidity Burn, Social Media Setup       |
| Phase 2   | CoinGecko Listing, CoinMarketCap Application           |
| Phase 3   | Website Launch, Whitepaper Publication                 |
| Phase 4   | Community Growth, Airdrop Campaigns                    |
| Phase 5   | CEX Listings, Strategic Partnerships, Merchandise Drop |
| May 2025  | Burn Additional 10 Billion Tokens                      |
| June 2025 | Register SPACEDOGE Logo with Etherscan                 |
| July 2025 | Listing with 3 Major Centralized Exchanges (CEXs)      |

---

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

* **Website:** [https://spacedoges.xyz](https://spacedoges.xyz)
* **Twitter:** [https://twitter.com/spacedogexyz](https://twitter.com/spacedogexyz)
* **Telegram:** [https://t.me/spacedogexyz](https://t.me/spacedogexyz)
* **GitHub:** [https://github.com/jewelpopri](https://github.com/jewelpopri)

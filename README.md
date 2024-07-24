# Swisstronik Tesnet 2.0 // Techinal Task 02.

Link : [Click!](https://www.swisstronik.com/testnet2/dashboard)

## Steps

### 1. Clone Repository

```bash
git clone https://github.com/sanztiva/SwisstronikERC20.git
```

```
cd swisstronik-erc20-mint-token
```

### 2. Install Dependency

```bash
npm install
```

### 3. Set .env File

create .env file in root project

```bash
PRIVATE_KEY="your private key"
```

### 4. Create Smart Contract

- Open contract folder
- Create Hello_swtr.sol file
- Copy this code and paste there

```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract TestToken is ERC20 {
    constructor()ERC20("PortToken","PORT"){}

    function mint1000tokens() public {
        _mint(msg.sender,1000*10**18);
    }

    function burn1000tokens() public{
        _burn(msg.sender,1000*10**18);
    }

}
```

### 5. Compile Smart Contract

```bash
npm run compile
```

### 6. Deploy Smart Contract

```bash
npm run deploy
```

### 7. Mint Token

```bash
npm run mint
```

### 8. Check Supply

```bash
npm run check-supply
```

### 9. Check Balance

```bash
npm run balance-of
```

### 10. Transfer Token

```bash
npm run transfer
```

### 11. Finsihed

Github  : [sanztiva](https://github.com/sanztiva)

Address Testnet Swisstronik 0x499da0675ddAE1589c6A4FC9BD6E254b4E8844dB
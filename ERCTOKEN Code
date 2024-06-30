// SPDX-License-Identifier: MIT
pragma solidity ^0.8.13;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.0.0/contracts/token/ERC20/ERC20.sol";

contract Cutekittens is ERC20 {
    constructor() ERC20("Ethereum", "ETH") {
        // Mint 100 tokens to msg.sender
        _mint(msg.sender, 200 * 10**uint(decimals()));
        //Similar to 1 Rupee = 100 paise
        //1 token = 1*(10**decimals)
        
        // Burn 100 tokens from msg.sender
        _burn(msg.sender, 100 * 10**uint(decimals()));

    }
}

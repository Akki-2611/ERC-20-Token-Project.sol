# ERC-20-Token-Project
This contract is written in Solidity, a programming language specifically designed for building smart contracts on the Ethereum blockchain.
# Description
This is a basic implementation of an ERC20-like token on the Ethereum blockchain. It leverages the standard ERC20 functionalities for minting, burning, and tracking total supply and individual balances. This demonstrates how to create and manage a token on the blockchain. You can use this contract to mint new Kitty tokens, distribute them to users, and even allow users to burn their tokens.

## Getting Started
## Executing program
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., ERCToken.sol). Copy and paste the following code into the file:

    // SPDX-License-Identifier: MIT
    pragma solidity ^0.8.13;

    import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/v4.0.0/contracts/token/ERC20/ERC20.sol";

    contract Cutekittens is ERC20 {
        constructor() ERC20("Ethereum", "ETH") {
            // Mint 100 tokens to msg.sender
            _mint(msg.sender, 200 * 10**uint(decimals()));
        
            // Burn 100 tokens from msg.sender
            _burn(msg.sender, 100 * 10**uint(decimals()));

        }
    }

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.18" (or another compatible version), and then click on the "Compile HelloWorld.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "Cutekittens" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the minting and burning function. Click on the "Cute_Kitten_Token"  contract in the left-hand sidebar. Call the Mint function with the recipient's address and desired amount. Click transact. After that call the burn function with the address to burn from and the amount. Click transact. Use the "balanceOf" function to retrieve the balance of any address. And other functions are given on the left-hand side. You can transact them.  It showcases how to inherit functionalities from the ERC20 standard and utilize functions for minting and burning tokens.
## License
This project is licensed under the MIT License.
## Acknowledgments
- Inspired by the ERC-20 token standard.
- Developed using Solidity and Ethereum tools.
  
Feel free to reach out for any questions or suggestions for improvement!

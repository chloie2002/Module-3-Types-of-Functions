# Module-3-Types-of-Functions

This Solidity program is a simple "Hello World" program that demonstrates the basic syntax and functionality of the Solidity programming language. The purpose of this program is to serve as a starting point for those who are new to Solidity and want to get a feel for how it works.

## Description
This Code Types of Function ETH + AVAX is to build your own  ERC20 token that enables the funtions and it should be burned and transferred by any user, but they can only be minted at a designated address. 

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

```javascript
pragma solidity ^0.8.0;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract CRUZCreateMintToken is ERC20 {
    address private  owner;

    constructor(string memory _name, string memory _symbol,uint256 initialSupply) ERC20(_name, _symbol) {
     _mint (msg.sender, initialSupply);
     owner = msg.sender;
    }
```

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4" (or another compatible version), and then click on the "CRUZCreateMintToken.sol" button.

Once the Code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "MyToken" and you will see the deploy and you will see the 3 parameters which is _Name_Symbol_InitialSupply once done click transact Scroll down you will see Deployed/Unpinned Contracts click "MyToken" you will see 7 variable which is approve,burn,mint,Transfer,Transfer open them once done click approve copy the first account in "ACCOUNT" copy the first account once done paste it in the Approve then the value is 5000 click transact and go open TotalSupply,Symbol,Owner,Name you will see in the TotalSupply is 5000 then click burn i place 500 and click TotalSupply as you can see the current value of050000by burning 500 the total value of my TotalSupply is 4500 next is Mint copy the second account from the "Account" Section then paste it in the Mint then the value is 500 and go again to the totalsupply to check if the value has been change as you can see it increase the current TotalSupply next one is transfer in the transfer section paste the second account and the value is 500 and go to the balanceOf to check any changees as you can see it the total amount is 4000 once done go to transferFrom paste the first Account in the from section then the 2nd Account paste the second Account to the "To" section and the ammount is 500 once done click allowance and paste the first account to the 2 blank wich is owner spender then click call the total Allowance of my account is 4000 and thats all thank you

## Authors
Chloie Jane T. Cruz 8215697@ntc.edu.ph

## License

This project is licensed under the MIT License - see the LICENSE.md file for details

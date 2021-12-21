```
pragma solidity ^0.8.0;

import "https://raw.githubusercontent.com/OpenZeppelin/openzeppelin-contracts/master/contracts/token/ERC20/ERC20.sol";

contract amalconrtacrt is ERC20 {

    constructor (string memory name, string memory symbol) ERC20(name, symbol){
         _mint(msg.sender,10**30);


    }

}
```
![screen](https://www2.0zz0.com/2021/12/21/08/204396809.png)
![screen](https://www2.0zz0.com/2021/12/21/08/543460271.png)


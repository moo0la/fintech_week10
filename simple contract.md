```
ragma solidity ^0.8.0;

contract EmptyContract {} 
  
contract Name {

    string public massage;

    constructor (string memory massage) {
        massage = massage;
    }
}
contract Bank{ 
   mapping (address=> uint) account_balances;

    function transfer (uint amount, address acctToTransferTo) external {

     

     account_balances[msg.sender] -= amount;
     account_balances[acctToTransferTo] += amount;
    }

    function bankBalance() external view returns (uint) { return address(this).balance;}

    }

    function withdraw(uint amount) external {

        account_balances[msg.sender] -= amount;
        payable (msg.sender).transfer(amount);
    }

    receive external payable {

        account_balances[msg.sender] += massage.value;
    }
```
![screen](https://www4.0zz0.com/2021/12/21/07/833995695.png)
![screen](https://www4.0zz0.com/2021/12/21/07/495644450.png)
![screen](https://www4.0zz0.com/2021/12/21/07/574916773.png)
![screen](https://www4.0zz0.com/2021/12/21/07/973769615.png)
![screen](https://www4.0zz0.com/2021/12/21/07/480998070.png)
![screen](https://www4.0zz0.com/2021/12/21/07/574916773.png)

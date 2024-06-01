# ETH_Beginner_proof
####This solidity smart conract will enable the smart contract to handle errors in a much more efficient manner.
copy these code snippets to run the program

this is the initialization of the contract and a variable.
```
// SPDX-License-Identifier: MIT

pragma solidity 0.8.25;

contract Rudra_error_handelling{

    uint public count=0;
```

this is the require function

```
 function mine_Require(uint supply) public{
        require(supply > 2000,"supply  greater than 2000");
        count++;
    }
```

this is the revert function
```
 function mine_Revert(uint supply) public {
        if(!(supply > 2000)){
            revert("supply should be greater than 2000");
        }
        count++;
    }
```

this is the assert funstion
```
function mine_Assert(uint supply) public{
        assert(supply > 2000);
        count++;
    }
    }
```
made with ❤️

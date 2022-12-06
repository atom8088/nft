pragma solidity ^0.5.0;

import "https://github.com/OpenZeppelin/openzeppelin-solidity/contracts/token/ERC721/ERC721.sol";

contract atom8088 is ERC721 {
  string public name = "atom8088";
  string public symbol = "ATOM";
  uint256 public totalSupply = 8088;

  constructor() public {
    // 初始化totalSupply个token的所有权
    for (uint256 i = 0; i < totalSupply; i++) {
      _mint(msg.sender, i);
    }
  }
}



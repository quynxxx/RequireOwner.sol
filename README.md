# RequireOwner.sol
RequireOwner.sol
pragma solidity ^0.8.20;
contract RequireOwner {
    address public owner = msg.sender;

    function check() public view {
        require(msg.sender == owner, "Not owner");
    }
}

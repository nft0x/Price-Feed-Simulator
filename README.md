# Price-Feed-Simulator
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract PriceFeed {
    uint256 public price = 2000 * 10**8; // giả lập giá ETH = 2000 USD

    function updatePrice(uint256 newPrice) public {
        price = newPrice;
    }

    function getPrice() public view returns (uint256) {
        return price;
    }
}

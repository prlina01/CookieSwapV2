# CookieSwap V2

**CookieSwap V2** is fully inspired by Uniswap V2.

### Main improvements from CookieSwap V1: 
* Any ERC20 token can be pooled directly with any other ERC20 token.  
* The introduction of ERC20 token/ERC20 token pools in CookieSwap V2 can be useful for liquidity providers, who can maintain more diverse ERC20 token denominated positions, without mandatory exposure to ETH.  
* Having direct ERC20/ERC20 pairs can improve prices because routing through ETH for a swap between two other assets (say, DAI/USDC) involves paying fees and slippage on two separate pairs instead of one.

![uniswapv2](https://user-images.githubusercontent.com/36077702/163624543-a2fa8331-eb9f-4378-8c42-760c11f4328e.jpg)
*_Source: https://docs.uniswap.org/protocol/V2/concepts/protocol-overview/how-uniswap-works)_

### Features
* **Pair contract** _(low level)_: Adding and removing liquidity, token swapping, price oracle with _time-weighted average price_ algorithm, UQ112.112 numbers.
* **Factory contact**: Generate and store token pairs, eip-1014(CREATE2 opcode).
* **Router contract** _(high level)_: Serves as the entrypoint for most user applications. This contract makes it easier to create pairs, add and remove liquidity, and perform actual swaps.
* **Library contract**: Calculates the swap amount. 

**To be continued...**

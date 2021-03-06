# UniswapV2 - Sushiswap version

## UniswapV2ERC20

![](https://raw.githubusercontent.com/knyumatt/solidity-contract-studies/master/sushiswap/graph/uniswapv2/UniswapV2ERC20.svg)

## UniswapV2Factory

![](https://raw.githubusercontent.com/knyumatt/solidity-contract-studies/master/sushiswap/graph/uniswapv2/UniswapV2Factory.svg)

## UniswapV2Pair

![](https://raw.githubusercontent.com/knyumatt/solidity-contract-studies/master/sushiswap/graph/uniswapv2/UniswapV2Pair.svg)

## UniswapV2Router02

![](https://raw.githubusercontent.com/knyumatt/solidity-contract-studies/master/sushiswap/graph/uniswapv2/UniswapV2Router02.svg)

# 

# Uniswap V2 Area

Code from [Uniswap V2](https://github.com/Uniswap/uniswap-v2-core/tree/27f6354bae6685612c182c3bc7577e61bc8717e3/contracts) with the following modifications.

1. Change contract version to 0.6.12 and do the necessary patching.
2. Add `migrator` member in `UniswapV2Factory` which can be set by `feeToSetter`.
3. Allow `migrator` to specify the amount of `liquidity` during the first mint. Disallow first mint if migrator is set.

To see all diffs:

```
$ git diff 4c4bf551417e3df09a25aa0dbb6941cccbbac11a .
```
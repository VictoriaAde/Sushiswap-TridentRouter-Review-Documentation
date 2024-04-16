# TridentRouter Contract Review Overview

This document provides an overview of the TridentRouter smart contract and its functions, along with a link to the detailed contract review documentation.

## Overview

TridentRouter is a smart contract designed to facilitate swapping tokens across Trident pools. It acts as a router, enabling users to execute various types of token swaps, add liquidity to pools, burn liquidity tokens, recover mistakenly sent tokens, and perform other related operations.

## Contract Functions

The TridentRouter contract provides several functions to perform different tasks:

1. **exactInputSingle**: Swaps token A to token B directly, using `bento` tokens.
2. **exactInput**: Swaps token A to token B indirectly by using multiple hops.
3. **addLiquidity**: Adds liquidity to a pool by depositing tokens and minting liquidity tokens.
4. **burnLiquidity**: Burns liquidity tokens to retrieve tokens from the pool.
5. **sweep**: Recovers mistakenly sent tokens from the contract.
6. **unwrapWETH**: Unwraps the contract's WETH tokens into ETH.
7. **deployPool**: Wrapper function to allow pool deployment to be batched.
8. **approveMasterContract**: Wrapper function to allow setting master contract approval to be batched.
9. **harvest**: Calls BentoBox harvest function to rebalance a BentoBox token strategy.
10. **exactInputSingleWithNativeToken**: Swaps token A to token B directly, depositing raw ERC-20 tokens into `bento`.
11. **exactInputWithNativeToken**: Swaps token A to token B indirectly by using multiple hops, depositing raw ERC-20 tokens into `bento`.
12. **complexPath**: Swaps multiple input tokens to multiple output tokens using multiple paths, in different percentages.
13. **burnLiquiditySingle**: Burns liquidity tokens to retrieve tokens from the pool in a single token.

Each function has specific parameters and functionalities, detailed in the contract documentation.

## Detailed Contract Review

For a detailed review of the TridentRouter contract, including line-by-line explanations of each function and its implementation, please refer to the [TridentRouter Contract Review Documentation on GitBook](https://vickish.gitbook.io/sushiswap-tridentrouter-review).


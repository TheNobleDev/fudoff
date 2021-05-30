# FUDOFF Audit Report

## Tokenomics
✅ Supply: 100 Billion
✅ Decimals: 9
✅ Total tax: 11%
* ✅ Holders: 1%
* ✅ LAto Liquidity: 4%
* ✅ Redistribution to wallets: 6%
    - `0xFefc71ab50c01DCCfB6Bd6270460a16BFbc4e9Cd`: 4%
	- `0x6f56477fa19CFBC3CB606FeA35A7B37CBDb2f444`: 2%

✅ Max transaction amount: 10 Billion
✅ Token balance to trigger Liquidity swap: 0.05% of total supply

## Testing

✅ Contracts compiled successfully.

The pancakeswap router address used is `0x10ED43C718714eb63d5aA57B78B54704E256024E`, which is the PCS Router v2 address.

* `_transferBothExcluded` works as expected, in case both sender and reciever are excluded from fee. 
* `_transferStandard` works as expected, in case none of sender and reciever are excluded from fee. 
* `_transferToExcluded` works as expected, in case only the reciever is excluded from fee. 
* `_transferFromExcluded` works as expected, in case only the sender is excluded from fee. 

## Suggested Feature Additions

It is suggested to add a new function, `excludeFromTxLimit(address account)` to allow certain addresses to make a large volume transfer of tokens, without their transaction failing.

## Important Notes

⚠️ The dead address (`0x000000000000000000000000000000000000dEaD`) is excluded from reward calculation, so it doesn't get any tokens from redistribution. Please ensure this is a requirement.

The owner has the priviledge to make the following changes:
* Change wallet addresses that get the 4% and 2% fee from every transaction. The ratio of fee can also be changed.
* exclude an address from fee
* include an address in fee
* set Tax Fee Percent
* set Liquidity Fee Percent
* set Max Tx Percent
* set/unset Swap And Liquify

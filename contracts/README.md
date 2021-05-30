
# Tokenomics


- Name: `FUDOFF`

- Symbol: `FUDOFF`

- Supply: 100 Billion

- Decimals: 9

- Total tax: 11%

- Holders: 1%

- Liquidity: 4%

- Wallets: 6%

- wallets addresses:

	- `0xFefc71ab50c01DCCfB6Bd6270460a16BFbc4e9Cd`: 4%

	- `0x6f56477fa19CFBC3CB606FeA35A7B37CBDb2f444`: 2%

- Max transaction amount: 10% (of total supply)

- Contract token balance to trigger liquidity swap + send to wallets: 0.05% (of total supply)

  
  

# Deploy

  

- Go to https://remix-alpha.ethereum.org/

  

- Change network to BSC in Metamask

  

- Change to address that has BNB in Metamask

  

- Create new file called `FUDOFF.sol`

  

- Copy and paste `contracts/FUDOFF.sol` into this file

  

- in the left sidebar go to SOLIDITY COMPILER

  

- Change to `v0.6.6`

  

- Check "Enable optimization". Leave "runs" at 200

  

- Click "Compile"

  

- in the left sidebar go to DEPLOY & RUN TRANSACTIONS

  

- Change ENVIRONMENT to Injected Web3

  

- Change ACCOUNT to the same account in MetaMask

  

- Change CONTRACT to `FUDOFF - FUDOFF.sol`

  

- Click Deploy

  

- Wait for deployment on BSC.

  

  

# Verify

  

- copy deployed address to clipboard

  

- go to https://bscscan.io/address/{ADDRESS}

  

- Click Contract > Verify & Publish

  

-  `Please select Compiler Type` > Solidity (Single File)

  

-  `Please select Compiler Version` > 0.6.6

  

-  `Please select Open Source License Type` > No License (None)

  

- Continue

  

- Optimization > Yes

  

- Paste in `FUDOFF.sol`

  

- Complete Capctha, done.
# Crypto FAQ for plebs!
Updated: 21 August 2021. Please DM [@deepseafarer](https://twitter.com/deepseafarer) on Twitter if you have any questions!

## Ethereum

#### What are the current L2 solutions that have been deployed?
Polygon and Optimism. There are many L2 solutions currently being developed that may be launched in the near future. For further details please check out this wonderful [tweet](https://twitter.com/GSpasov/status/1426915044307132418) by George!

#### What is the mempool?
The mempool is a set of broadcasted transactions that have not been added into the blockchain. Miners decide which transactions to validate and include in the block, and often select transactions with higher fees.

#### How do I transfer cryptocurrency to the Polygon L2?
The easiest way is to first add the Polygon Mainnet on your Metamask wallet. Please do so by following the instructions [here](https://docs.matic.network/docs/develop/metamask/config-polygon-on-metamask). After doing so, use the [Polygon bridge](https://wallet.matic.network/bridge) to transfer your assets on the Ethereum blockchain over to the Polygon blockchain. Be careful when choosing any blockchain bridge to transfer your assets, as some bridges may be vulnerable to hacks or are malicious!

#### What is wETH?
wETH is short for wrapped ETH, and is different from the native token of the Ethereum blockchain, Ether (ETH). wETH is ERC20 compatible, which allows it to be handled by smart contracts. Many decentralized applications (dApps) use wETH in place of ETH, so care should be taken to note which token you are dealing with.

## DeFi

#### What is yield farming?
Yield farming is a catch-all term referring to the practise of earning yields on cryptocurrency a user holds. It is similar to receiving interest on bank deposits. For cryptocurrency, yield can be received in terms of the cryptocurrency provided, or in terms of the protocol's native token. In particular, the practise of receiving a protocol's native token for providing liquidity to the protocol is known as liquidity mining.

#### What is liquidity mining?
Liquidity mining refers to the issuance of native tokens by protocols to liquidity providers (LPs). For example, LPs that deposit ETH-USDC to liquidity pools on Sushiswap are rewarded with the native token $SUSHI. Protocols typically issue tokens to incentivize people to provide liquidity to their liquidity pools. Issuance of tokens is commonly very high in the beginning as protocols seek to bootstrap liquity in early pools (i.e. incentivise people to start depositing cryptocurrency into a pool).

#### Where do yields in DeFi come from?
There are many types of yield in DeFi. It is important to identify how protocols generate yields (i.e. how protocols generate value) in order to decide whether they are sustainable or not. Below is a breakdown of the main types of yields in DeFi:
1. **Proof of stake**: Protocols issue rewards for stakers that stake cryptocurrency to validate the blockchain. E.g. ETH2.0
2. **Lending**: Borrowers pay interest for loans. E.g. Aave, Compound
3. **Protocol usage**: An excellent example is the trading fees that DEXs charge users. E.g. Uniswap, Sushiswap
4. **Protocol-issued incentives**: An excellent example would be liquidity mining, where protocols reward early liquidity providers (LPs) with native tokens. E.g. Compound
5. **Products and services**: Protocols sell financial products such as insurance or covered calls or puts. E.g. Nexus Mutual, Dopex

#### Which DeFi protocols are live on Ethereum L2 platforms?

| L2 platforms | Protocols |
| ----- | ----- |
| Polygon    | 1inch <br> Aave <br> Balancer <br> Curve <br> Sushiswap |
| Optimism   | 1inch <br> Synthethix <br> Uniswap |

#### What are stablecoins?
Stablecoins are cryptocurrencies that are pegged to the value of fiat currencies such as the US dollar. Examples of stablecoins are Tether (USDT), USD Coin (USDC), DAI and Binance USD (BUSD). Stablecoins must fulfil token standards of their respective L1 blockchain. For examples, stablecoins on the Ethereum blockchain are ERC-20 tokens. The same stablecoins are not transferrable across different L1 blockchains (i.e. cannot send USDC from an Ethereum wallet to a Solana wallet).

<!-- #### What is impermanent loss?

#### What are the main uses of DeFi?

#### What is an automated market maker?

#### Are impermanent losses the same on all AMMs?
No. Depends on the maths behind the liquidity pools.

#### Do I have to place equal assets in Balancer pools?

## DeFi protocols
### Aave
Aave is a lending protocol.

### Balancer
Balancer is an AMM

### Quickswap -->

---
layout: default
---

# Terra - DeFi

## Mirror
[Mirror](https://mirrorprotocol.app/#/trade) is a DApp that enables the creation and trading of synthetic assets that track the price of real-world assets such as stocks. These synthetic assets are termed Mirrored Assets (mAssets), with examples being mAAPL, mGOOGL and mAMZN. International users that have trouble owning US stocks can now gain exposure to the price movements through these mAssets.

Prices of mAssets are determined by their prices on the Terraswap AMM (which is determined from the composition of the liquidity pool), and may deviate from the real-time prices of their underlying assets. In Mirror, real-time prices are provided by price oracles (Band Protocol), and both the oracle price and the price premium of the mAssets are reported. 

mAssets are minted/created through a process termed as short farming. Collateral is first provided in the form of aUST or UST, and the desired mAsset can be borrowed/minted against the collateral at a specified collateral ratio. For example, a collateral ratio of 200% would mean that the provided collateral would have to be twice the value of the underlying asset. When the mAsset is minted, it is immediately sold at the Terraswap price, with the user getting the sale proceeds after a locking period of 2 weeks. The initial collateral can be redeemed by repurchasing the quantity of mAsset minted and burning it. Mirror rewards you for taking a short position by issuing you $MIR (hence the term short farming).

#### How do mAssets keep their peg to their underlying assets?
Mirror relies primarily on minting liquidations and arbitrageurs to keep mAsset prices close to their real prices. Minting liquidation is triggered when the oracle price of the mAsset increases till the point when the collateral ratio of the minted mAsset falls below the minimum collateral ratio (MCR) of 150%. Mirror will automatically sell collateral to buy the mAsset until the collateral ratio reaches the MCR. The bought mAsset is automatically burned to repay the minted mAsset (without any return of collateral). This creates buy pressure for the mAsset, driving the Terraswap price higher. Arbitrageurs can profit by buying mAssets when they are undervalued and minting (and selling) mAssets when they are overvalued, with the expectation that prices will converge to the oracle price.

#### How do I farm 30%+ APR on stablecoins?
Farming a yield of 30%+ APR using stablecoins can be done by engaging in both long farming and short farming on Mirror, with the help of [Anchor Protocol](https://app.anchorprotocol.com/)! Long farming is essentially providing liquidity of an mAsset-UST pair, liquidity providers will be rewarded with $MIR. Short farming is essentially minting (and selling) an mAsset, and is described in detail above.

This delta-neutral strategy is described in detail on <https://mirrortracker.info/>, as the "Short, Long Buy Neutral" strategy. The website also reports 30 Day average Long Farm and Short Farm APRs.

A word of warning when employing this strategy. Be careful of minting liquidations and impermanent loss! An increase in mAsset price might trigger a liquidation on your short farm when MCR goes below 150%! In addition, if mAsset increases/decreases in price you will suffer from impermanent loss! For example, when mAsset increases in price you will get back a lesser quantity of mAsset which the corresponding increase in UST will not compensate fully for. If price of mAsset goes down, you will end up with a larger quantity of mAsset but a smaller amount of UST.


## Anchor Protocol
[Anchor Protocol](https://app.anchorprotocol.com/) is the money market (or lending) protocol on Terra. Depositors are able to deposit UST to obtain an APY of 20%, or bond $LUNA/$stETH to obtain $bLUNA/$bETH. Holders of $bLUNA and $bETH, whether it be a wallet address or smart contract (e.g. Anchor collateral smart contract), are entitled to staking rewards. However, $bLUNA holders are not entitled to airdrops that are distributed to $LUNA stakers.

Users are also able to deposit their $bLUNA/$bETH as collateral into Anchor to borrow $UST, while getting charged a borrow APR. Currently, most of the borrow APR is offset by Anchor distributions of their native $ANC token.

#### How is Anchor able to sustain its yield at \~20%?
Anchor seeks to provide a long-term stabilised yield rate, which is currently decided upon through governance to be at \~20%. In the future, this yield rate may decrease. Anchor has two main income streams in order for it to sustain its deposit APY:

1. Borrow APR that it charges lenders
2. Yield from deposited collateral of PoS tokens (e.g. $bLUNA, $bETH)

In the event that Anchor does not earn enough yield to cover its target yield rate, Anchor will draw from its $UST yield reserve. The yield reserve was funded initially by Terraform Labs. When Anchor earns in excess of its target yield rate, the excess yield rate will be deposited into the yield reserve.

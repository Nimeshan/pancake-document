# FAQ

### Why are there multiple APRs?

In V3, you can concentrate your assets while providing liquidity to boost your share against the total available liquidity, earning a higher % of rewards.&#x20;

Therefore, depending on the position price-range settings, each liquidity position will have its own LP fee APR and its own farming APR.

The global APR is calculated with the total amount of CAKE rewards in USD, divided by the total amount of assets, with in the active positions, which are currently staked in the farm. So, global farming APR is only a generic reference, and will not represent individual APRs for each positions.

To view your farming APR, check out your positions listed under each farm.

###

### What happens if my liquidity position goes out of range while staking in the Farm?

In V3, only active (in-range) liquidity positions will earn CAKE from farms.

The position will stop receiving CAKE rewards when the price goes out of the range.

If the price moves back in range, the position will start receiving CAKE rewards again. No additional actions are required from stakers.



### Are there any ways to automatically adjust my position so it is always in range and earning fee rewards?

Automatic position managing feature is coming soon to PancakeSwap v3 with one-click liquidity depositing (Zap!) and farming. Stay tuned for more detail.



### Is it better to always farm with a liquidity position with a smaller range?

Providing liquidity to a smaller price range will help concentrate your liquidity, boosting your relative shares again the total liquidity within the price range, potentially earning more CAKE rewards.

However, please bear in mind that only active liquidity positions will earn CAKE rewards. This means you will only earn rewards when the current trading price is within the price range defined in the liquidity position.

If you need to adjust your position price range, you will need to unstake, remove liquidity and create a new position with the updated price range. Please bear in mind that frequent adjustments are not always the most optimal strategy as it realises the impermanent loss and costs a certain amount of gas to complete multiple transactions.



### How many positions I can stake in one single farm?

There is no maximum limit of positions you can stake in one farm.

But please bear in mind that you will need to spend gas to manually harvest from each one of the positions. Please always factor gas cost in the yield operations.



### How often should I harvest my rewards?

How often you harvest your rewards is up to you, but it does help to remember that there is a small fee involved in harvesting. You can see this fee in your wallet when confirming after clicking “Harvest”**.**

This shows the fee for harvesting as it appears in the MetaMask wallet. Different wallets will show the information a little differently. Consider leaving your rewards to grow for a while so you pay fees less often.



### What if I want to adjust my position while staking in the farm?

While staking in the farm, you are able to add or remove liquidity without unstaking it. Simply locate the liquidity position you want to adjust, and click its title/id, and you should be presented with the position detail page where you can use the “Add” and “Remove” buttons.

If you want to adjust the price range configurations of a liquidity position, you will need to unstake it from the farm, remove all liquidity and re-create a new position by adding liquidity.



### What affects Farming APR?

In Farm v3, CAKE reward APR could vary between liquidity positions. It is based on the following factors:

* CAKE emission rate to Farms\
  \- more CAKE will generate a higher yield for all the farms. Read more on [our tokenomics page](https://docs.pancakeswap.finance/tokenomics/cake/cake-tokenomics)
* Farm multiplier\
  \- farms with a higher multiplier will get more CAKE proportionate to all the farms. Please note that v3 and v2 + stable swap farms are using two separate sets of multipliers. And farms on Ethereum and BNB Chains are also using two separate sets of multipliers.
* The number of tokens deposited in the position\
  \- more token in the position translates to a larger relative share against the total active liquidity in the farm pool and gets more CAKE rewards
* The selected price range\
  \- smaller price range allows a higher concentration for the same amount of token deposited, which translates to a larger relative share against the total active liquidity in the farm pool, and gets more CAKE rewards
* The amount of liquidity currently active\
  \- if there are more users who deposit and concentrate their liquidity with the same range as you, you will earn CAKE rewards due to a smaller relative share against the total
* Whether the liquidity position is active\
  \- only active liquidity positions will earn CAKE rewards from farm



### Why am I seeing an "Update Positions" pop-up?

![](<../../.gitbook/assets/image (321).png>)

Soon after the V3 launch, Chefs implemented an update on Farms to make reward calculations more accurate and reliable. If you are seeing this pop-up, that means some of your positions will require an update.

Simply click "Update All", and confirm in your wallet pop-up.

Please note that Chefs are also applying this update to the historical staking data between the launch of Farm V3 and when this update is implemented. If there are any extra CAKE rewards, they will be airdropped to your wallet before 1st May 2023.



### Why a 2x farm in V3 has less APR than a 1x farm in V2?

First, when comparing APRs, you need to ensure the total staked liquidity between two farms is equal.

On top of that, we now have multiple groups of farms which have their own stream of CAKE emissions. And each group of farms shares separated sets of multipliers.

An individual farm will receive CAKE emissions based on:

* A = Total CAKE per second/block for the farm group it belongs to
* B = Total number of multipliers within the group it belongs to
* C = The multiplier has

`CAKE per block/second = C / B * A`

The above numbers can be found in each of the [MasterChef](../../developers/smart-contracts/main-staking-masterchef-contract/) contracts.



### Can I use bCAKE in v3 Farms?

Yes

bCAKE for V3 Farms will come very soon after the deployment of PancakeSwap Farm V3. Stay tuned.

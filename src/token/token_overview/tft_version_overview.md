								
# TFT Versions

|		|	version 1 Rivine	|	version 1 Stellar	|	version 2 Stellar	|
| --- | --- | ---	| ---	|
|	blockchain tech	|	Rivine, proof of blockstake	|	Public, Stellar	|	Public, Stellar	|
|	on public blockchain	|	march 2018	|	2020 May	|	2020 May	|
|	farmed since	|	+-2017	|	2020 May	|	tbd	|
|	freely transferable (*)	|	YES	|	YES	|	YES	|
|	complete blockchain featureset	|	YES	|	YES	|	YES	|
|	decentralized exchange	|	YES (atomic swap)	|	YES (Stellar)	|	YES (Stellar)	|
|	public exchange	|	BTC Alpha	till Dec 2019|	Stellar	|	BTC Alpha & Liquid	|
|	freely tradable on exchange	|	YES	|	YES	|	YES	|
|	min price (price protection)	|	NO	|	NO	|	YES	|
|	Name on Blockchain	|	TFT	|	TFTA	|	TFT	|

So basically the only difference between v1 & v2 is that TFTv1 can not be sold on the public exchange if the price is lower than $0.15 + 2% per month starting may 2020. This has been implemented by creating 2 trustlines on Stellar and making sure that no-one can sell lower than the min price. 

2 methods have been implemented to achieve price protection for TFTv1 to TFTv2

- appointed 3e party independent market maker (used by Foundation uses, anyone else can as well, there are costs related to this)
- the TF [market maker bot](threefold_marketmaker_bot), see below

## migration

### migration from TFTv1 Rivine to TFTv1 Stellar

- by means of blockchain operation done by the user of wallet.
- the most userfriendly way was by means of ThreeFold Wallet as part of 3bot connect.
- every user had to do the transaction themselves, no developer or anyone else had control over this migration step.

#### Status July 2020

- almost all TFTv1 have been migrated.
- Any user could do this migration started May 2020
- there has been a bug in 3bot connect which caused a visualization issue about amount of tokens in the 3bot connect UI.
- checking tools have been created and executed to check that every transaction happened appropriately and that exact amount of TFTv1 was same.

### migration from TFTv1 Stellar to TFTv2 Stellar

The community believes that price protection is good for everyone because the TFT is not a speculative token and has never been promoted as a speculative crypto currency. TFT represents capacity on the TF Grid.

We are at the stage of rolling out the TF Grid, there is a lot of capacity but not enough locations.

Starting July, every TFTv1 user can sell to Stellar/BTCAlpha/Liquid with price protection. For that they need to use a [market maker bot](threefold_marketmaker_bot).
After selling the person who bought the TFT receives automatically a TFTv2.

> Please note that we worked on this for about 12 months from out of the TF Foundation (ThreeFold FZC) and worked closely with our community. We did zoom calls to prepare and get required consensus. We also did a poll with our farmers to make sure we have consensus about this change. The huge majority of TFT v1 token holders agreed on making this change for the better good of the ThreeFold project. July 2020 the 2nd version of this poll is still ongoing. See: https://poll21.threefold.me/

> Please note, if the community would believe that this price protection is not needed the TF Foundation will suggest code changes which the developers can implement and the grid council can execute upon.


#### Status July 2020: 

- limited liquidity on the public exchanges, this means most users who want to sell will not find the liquidity yet. TF has planned more marketing activities to improve the liquidity situation.


#### Status TDE

The Foundation is organizing a TDE = [Token Distribution Event](token_overview_tde.md) and has raised +1m USD for this event.
This funding allowed the onboarding of Liquid exchange and the marketing & promotion efforts of last 12 months as executed in TF Foundation. Our original idea was to raise money for the TDE on liquid but this did not happen/work, the TF Foundation had 1 month priority on liquid to try and sell TFTv1, we used a 3e party marketmaker for this.
We are preparing our TDE for probably sept 2020. 



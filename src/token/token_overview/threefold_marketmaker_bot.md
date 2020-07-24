# Threefold Marketmaker Bot

The TF marketmaker bot is a digitized bot operated by the ThreeFold Foundation (ThreeFold FZC). 
The purpose is to allow the ThreeFold community to easily sell TFTv1 onto 3 public exchanges at once

- Stellar
- Liquid
- BTCAlpha

> IMPORTANT DISCLAIMER: <BR> 
> ThreeFold FZC is not taking any responsibility for any potential issue related to the usage of this sales bot. <br>
> The code of the Sales Bot is opensource and used as is by ThreeFold FZC <BR>
> By using this service you have read and accepted our terms & conditions [on this link](disclaimer.md).

In line with majority approval of the TFTv1 token holders, a price protection has been established till end 2020 to protect the interest of the ThreeFold community. If at any point in time majority of TF Community would want to remove this price protection then this code change will be suggested to the code developers and TF Technology council will approve the upgrade.

- Until the end of 2020 TFTv1 (TFTA) can only be sold on Liquid & BTCAlpha if the sell price is higher than the Min TFT price.
- Min TFT price is USD0 .15 starting April 29, going up 2% per month compared to the USD.


> At time of writing +90% of our community has voted for this price protection (see https://poll21.threefold.me) <BR>
> TFFoundation has done everything possible to make sure that NO TFTv1 (TFTA) holder can sell for prices lower than the minimum price. <BR>
> We would like to remind you that if you have not voted yet please do so, your vote is important.<BR>


### tutorial

![](img/mm_bot1.png)

![](img/mm_bot2.png)

![](img/mm_bot3.png)

Specify the amount of TFTv1 (TFTA) you want to sell on one of the exchanges.

![](img/mm_bot4.png)

Normally no need to fill this in, the XLM will be send to the wallet you have used to sell your TFTA from.

![](img/mm_bot5.png)

Once the tokens arrive the order has been done.

![](img/mm_bot7.png)

In this example we use the Solar wallet to send the tokens.

![](img/mm_bot8.png)

The order has been done.

If you go back to the bot you will see an overview screen with the open trade order.
You can at any point cancel the trade.

### remarks

- The sales orders are always done versus XLM which is the native Stellar currency
- This means if someone wants to buy TFT for BTC, it will still work, Stellar payments network will convert to XLM and then to TFT. 
- The sales on BTCAlpha and Liquid are always converted back to XLM.
- The name "marketmaker bot" might be misleading. This bot does not have funding to keep a market stable, this bot has as goal to allow any TFTv1 (TFTA) token holder to sell tokens to public exchanges easiest possible way while maintaining a minimum price.


> Important note: TFTs are not an investment instrument. TFT's are used to buy/sell IT Capacity.

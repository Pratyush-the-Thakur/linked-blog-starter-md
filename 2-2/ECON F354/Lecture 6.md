
### Uses
- hedge risks
	- hedgers
	- Say 20% of your portfolio is REL, you're unsure as to what will happen on the 25th
	- To protect yourself from falling prices, you can use a future contract to sell X amount at $Y.
	- Say you're a farmer, the price of wheat is very variable, you would rather a consistent amount of money than a variable one. You do the same
- speculate
	- Purely to make profit, nothing else
	- No asset exposure, or you dont really care about the underlying asset
	- But you do have some expectations on how the prices will change
	- If they'll rise, you take a long position, a short position if you expect them to fall
- lock in an arbitrage profit
	- Arbitrage Traders
	- Riskless profit
	- Say you expect the prices of REL to rise, you take a long position, but you could be wrong
	- How?
	- Magnitude is considerably smaller, and exists for a very small amount of time
	- Mispricing
	- Say a company X, its 2500 in the USA and 2300 in India, thats a 200 arbitrage (Exchange rates and stuff)
	- If no restrictions(which there are, you cant just buy a security in one market and sell it in another), instant 200, no risk at all
	- Mostly not for the common man, arbitrage traders use algorithms to instantly find and cash these in


### Options example

- say you have 2000
- $20 per stock, you expect it to go up
- A call option with a strike price of 22.50 is $1
- So you pay  $100 for the option
- 100$ spent
- Now, if the price per share crosses 22.5 (or a total of 2250 for you)
- You can buy 100 shares for it for 2250, no matter how much it exceeds 2250 by
- In this case, to break even, the stock would have to rise to 23.50 (2250 + 100)/100
- if the stock rises to $25, you can buy it for 2250, and immediately sell it in the market for 2500, instant 250 - 100(for the option) = $150 profit
- If you had done this in the spot market, and had just bought 100 shares for 2000, and sold it at 2500, you would have gotten $500. 
- Wait, isnt that more?
- It is, however, if the price fell to... say $1800, in the spot market, you would have lost 200, but in the derivative market, you would have only lost the option cost that you paid ($100). Since the strike price is 22.50


- Security is trading at 100
- Put Option trading at $2, strike price is $120
	- (basically, buying the right to sell the security)
- Bullish trader will sell put option as he expects it to go up

```
t = 0, given bullish expectations
Trader takes a short position, sells put option
Receive 2*100 = $200
K = $120

t = T

case 1: St = $150

buyer of the option will prefer to sell it at market price (AGAIN, THE TRADER IS NOT THE ONE WHO HAS BOUGHT THE RIGHT HERE, HE IS THE ONE WHO HAS SOLD THE RIGHT, VERY IMPORTANT)

you profit 200, because the guy basically paid you 200 for the right to sell it at a price, and just didnt exercise it

case 2: St = 110

buyer of the option will exercise his right to sell it at 120
-10*100 = -1000
You suffer losses  of 1000 - 200 (for the option)
-800

However, buyer also suffers losses, because even though he sells it for 120, he also spent 200 on the option itself, so his profit is only 1000, he could have just sold it for 1100 in the spot market

case 3: St= 80

buyer will exercise his right to sell at 120
-40*100 = -4000
you suffer losses of 3800

And the buyer does gain profits in this case, in the spot market, he would have only gotten 8000, here he's made 11000 (subtracting the option price), thats a $3000 profit

```
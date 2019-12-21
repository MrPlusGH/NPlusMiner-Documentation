![alt text](https://github.com/MrPlusGH/NPlusMiner/raw/master/Includes/NPM.png)
# Estimations and Projections
There are different notions that NPlusMiner uses to decide what to mine and show earnings. Both these values are different. This page is an attempt to clarify on this topic.

## Earnings tracking
### Balance
Values shown in Earnings Tracking are real values. The balance shown is the actual amount you made on the pool there is no estimation here.
   **Balance is the actual amount you already made.**
   
   **This is what you will be paid by the pool**
   
!! DO NOT select different variants of the same pool !!

     The BTC/Day value shown by NPlusMiner at the top of the window is the sum of what your making on all selected pools.
     Users must not select different variants of the same pool in config (Pool, Plus, 24hr).
        This defeats estimations principles and will give bad results.
     If done so, the sum will show wrong values.
   
   
### Projection
NPlusMiner look at the per hour growth of your **actual** earnings at the pools and deduces the BTC/day that you are actually making. From there, it does some calculations to determine the Estimated Pay Date **If this BTC/day is kept somewhat constant**.
The average is calculated from the last 1 day + 1hour (once the NPlusMiner instance get that runtime).
The Trust index percentage indicates how accurate these projections are.

## Estimations
To take decisions on which algo and which pool it should mine, NPlusMiner uses information provided by the Pools. **These are estimations and not real prices**.
It is basically an attempt to predict the future. No one can pretend being accurate when playing that game.
Still, this is an important piece of information used to take decisions.

**This is not what you will earn**.

When using Plus. NPlusMiner uses some advanced calculation based on different pool estimations to get more realistic estimates and be resistant to spikes in price.
It includes some Trust and Stability index based on past hour estimations variations.
So when using Plus, you rely on more realistic estimates, get less switching, better profitability.

***
Copyright © 2018 MrPlus


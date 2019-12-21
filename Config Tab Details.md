![alt text](https://github.com/MrPlusGH/NPlusMiner/raw/master/Includes/NPM.png)
# Config Tab Details

![alt text](https://github.com/MrPlusGH/NPlusMiner-Documentation/blob/master/NPMConfig.JPG)

## Mandatory settings
Below is the only mandatory setting for NPlusMiner.
Just type your address in (1) and hit Start (21)

1 - BTC Address

        Your BTC Wallet address

## Optional settings
2 - Worker name

        Name you want to see on the pool side for your rig (Not mandatory)
        
3 - MPH UserName

        Only used for MiningPoolHub. Your MiningPoolHub user name
        
4 - Interval

        This defines the NPlusMiner cycle. Default is NPlusMiner will check pools every 120 seconds or 2 minutes
        
5 - Location

        Preferred location for pools which supports it. Default is US if pool does not support the specified region.
        
6 - GPU Count

        Number of GPUs on your system. Click on "Detect GPU" (7) for NPlusMiner to detect it on its own.
        
7 - Disable GPU 0

        NPlusMiner will not use the first GPU found on the system. Could be used for gaming while mining.
        
7 - Detect GPU

        Detects the number of GPUs on the system
        
8 - Algorithm

        This defines the list of alforithm which NPlusMiner will actually mine. If you do not want to mine a specific algorithm, remove it from the list.
        Use the "Load default algos for selected pool" button (20) to load the default algo list for selected pools in (15)
        
9 - Currency

        Currency you want NPlusMiner to display
        
10 - Pwd Currency

        Currency you want to use at the selected pools when supported by the pool. Do not use if you do not understand.
        
11 - Donate

        Number of minutes of mining you will donate to developers per day. Default is 8. Minimum is 3. Setting anything lower than 3 will pick a random value from 0,3,4,5,6,7,8.
        
12 - Proxy

        Enter proxy address if you need to use a proxy. Leave blank if not.
        
13 - ActiveMinerGain%

        This defines the percent theshold for NPlusMiner to switch algo. If the best profit algo is less than x% above the current algo profit, NPlusMiner will not switch. Use to avoid high switching rate.
        
14 - MPH API Key

        Your MiningPoolHub API key used to fetch your balance on MPH by the Earnings Tracker.
        
15 - Pools

        Select the pools on which you want to mine. 
        
16 - Autostart

        Tells NPlusMiner to start mining after its launched. No need to press start button.
        
17 - Enable Tracker Log

        Will log earnings in \logs folder in csv format. Could be imported in Excel to track earnings progress.
        
18 - Start UI Minimized

        Minimzes the application window at start
        
19 - Save Config

        Self explanatory
        
20 - "Load default algos for selected pool"

        Will load the default algo list for selected pools in (15) into algorithm (8)
        
21 - Start / Stop button

        Starts or Stops NPlusMiner activities
        
22 - Pause / Mine button

        Pause will pause any mining activity while keeping Earning Tracker and BrainPlus jobs running. This avoids NPlusMiner learning curve when resuming mining.
        
23 - BTC/D

        Shows estimation of earning rate in BTC/D and mBTC/D
        
24 - Current mining activity

        Self explanatory
        
***
Copyright © 2018 MrPlus

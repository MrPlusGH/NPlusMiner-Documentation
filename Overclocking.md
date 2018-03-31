![alt text](https://github.com/MrPlusGH/NPlusMiner/blob/2.1/NPM.png)
# Overclocking
!Use OC with caution!

If overclocking, the overclocking settings need to be set before first run of NPlusMiner because of algorithm benchmarking.  If overclocking settings were changed after the benchmarking, you'll need to run the ResetBenchmark.bat batch file.

Gigabyte Xtreme Gaming Engine (VGA - XTREME ENGINE) is recommended for overclocking software.  In settings, there is a "Synchronize settings for similar graphics processors" option.
Note that it minimizes to the system tray.  To open, right click on the icon and select open.

VGA - XTREME ENGINE download:  https://www.gigabyte.com/Support/Utility/Graphics-Card

Recommended overclock settings for GeForce GTX 10 Series (1050 - 1080 Ti)
```
 Power: 70% - 80% (-30 - -20)
  Core: 0 - +50
Memory: +400 - +600
```

If a GPU is overclocked too high, there is a risk of crashing, freezing, and increase of bad shares.

For advanced overclocking, one can run algorithm specific overclocking by using NPlusMiner's Prerun feature and NvidiaInspector.  Make sure there isn't other overclocking software running.  Simply create a file named <AlgoName>.bat in the prerun folder.  If <AlgoName>.bat does not exist, NPlusMiner will try to launch prerun/default.bat.  There is a default-Example.bat file in the prerun folder that has example code in it.

```
Use case example 1:
Your Rig is showing issues with only one algorithm (say x16r) and you realize this guys needs different OC settings than others.
Create .\prerun\default.bat with the common OC settings for all algos.
Create .\prerun\x16r.bat with the specific OC settings for x16r.
NPlusMiner will now automatically change OC settings accordingly.

Use case example 2:
Your OC settings are sometimes going away when the GPU driver crashes.
Create .\prerun\default.bat with the common OC settings for all algos.
NPlusMiner will now automatically update OC settings each time it switches algo.
```

NvidiaInspector download:  https://github.com/Orbmu2k/nvidiaProfileInspector/releases

!Use OC with caution!

Copyright © 2018 Tesla74

Parameters:

```
  <I32 N="SampleSizeMinutes">60</I32>
        BrainPlus uses data from the last 60 minutes to perform its calculations.
        This setting defines the data sample size in minutes.
  <I32 N="Interval">60</I32>
        Defines the time interval between pool API polls. Default is every 60 seconds.
        Which gives 60 data points per sample.
  <I32 N="SampleHalfPower">0</I32>
        Could be used to introduce a ratio of power between Full sample size and Half sample size.
        0  - Use only full sample size data
        >0 - Gives more importance to most recent data than older ones in the sample data set.
  <B N="EnableLog">false</B>
        Enables logging. See LogDataPath.
        Ever wanted to visualize what BrainPlus is. Load the resulting csv in Excel and visualize price history.
  <S N="LogDataPath">.\BrainMemory-ahashpool.csv</S>
        Path to log file when logging is enabled. Defaults to .\BrainPlus\<PoolName> folder
  <S N="TransferFile">.\ahashpoolplus.json</S>
        File where NPlusMiner will read the resulting calculations to base switching decisions against.
        DO NOT CHANGE. 
  <S N="PoolName">ahashpool</S>
        Self explanatory
  <S N="PoolStatusUri">https://www.ahashpool.com/api/status</S>
        Pool API Uri which will be polled for prices at every defined Interval
  <I32 N="ManualPriceFactor">1</I32>
        Not used
  <I32 N="TrendSpanSizeMinutes">30</I32>
        Not Used



```

------

------

Copyright (c) 2018 MrPlus (https://github.com/MrPlusGH/NPlusMiner)
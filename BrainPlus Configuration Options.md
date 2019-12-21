![alt text](https://github.com/MrPlusGH/NPlusMiner/raw/master/Includes/NPM.png)
# BrainPlus Configuration Options
BrainPlus does not need any configuration tuning. Default settings have proven to be effective.

For users who like to play the tuning game, some settings could be modified using the BrainConfig.xml file found the correspondig .\BrainPlus\<PoolName> folder.

Parameters:

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





***
Copyright © 2018 MrPlus (https://github.com/MrPlusGH/NPlusMiner)

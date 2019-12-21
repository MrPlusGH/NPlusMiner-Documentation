![alt text](https://github.com/MrPlusGH/NPlusMiner/raw/master/Includes/NPM.png)
# NPlusMiner Features
*****

NPlusMiner Monitors mining pools in real-time in order to find the most profitable Algo

	 GUI and easy configuration
	 Auto Benchmarks Each algo to get optimal speeds 
	 Fully automated 
	 Auto Downloads Miners

*****

   GUI

      Since version 2.0 NPlusMiner has a GUI making it easy to configure and run.
      Relies on config files. No need to edit bat files. Simply run NPlusMiner (Not the .ps1) 
      Set the config on the config tab, save, close, run
      For console lovers. Right click the NPlusMiner file > Properties > change "hidden" to "maximized" in the target field

   Prerun

      Ability to run a batch prior switching to a specific algo.
      For example, can be used to set per algo OC via nvidiaInspector
      Simply create a file named <AlgoName>.bat in prerun folder
      If <AlgoName>.bat does not exist, will try to launch prerun/default.bat
      Use overclock with caution

   Per Pools Config (Advanced)

        - **This is for advanced users. Do not use if you do not know what you are doing.**
        - You can now set specific options per pool. For example, you can mine NiceHash on the internal wallet and other pools on a valid wallet. This configuration is provided as an example in Config\PoolsConfig-NHInternal.json
          - Available options
            - Wallet = your wallet address
            - UserName = your MPH user name
            - WorkerName = your worker name
            - PricePenaltyFactor = See explanation below
          - Usage
            - The file Config\PoolsConfig.json contains per pool configuration details. If a pool is listed in this file,
        the specific settings will be taken into account. If not, the setting for the entry name default will be used.
        **Do not delete the default entry.**
            - Edit Config\PoolsConfig.json
            - Add an entry for the pool you want to customize
              - The name must be the NPlusMiner name for the pool. ie. for ahashpool, if you use Plus. The name is ahashpoolplus.
              - (**careful with json formating ;)**)
              - Best way is to duplicate the default entry
        - Note that the GUI only updates the default entry. Any other changes need to be done manualy

   PricePenaltyFactor

        - When using advanced per pool configuration, it is possible to add a penalty factor for a specific pool. This simply adds as a multiplicator on estimations presented by the pool.
        - Example scenario
          - NiceHash as a 4% fee - Set PricePenaltyFactor to 0.96 (1-0.04)
          - You feel like a pool is exaggerating his estimations by 10% - Set PricePenaltyFactor to 0.9

   Earnings Tracking

      Displays BTC/H and BTC/D as well a estimation of when the pool payment threshold will be reached.
      Supported pools:
            ahashpool
            zergpool
            zpool
            nicehash
      If mining more that one pools, shows stats for any supported pool
      Press key e in the console window to show/hide earnings

   Algorithm Switching Log

      Simple algo switching log in csv switching.log file found in Logs folder.
      You can easily track switching rate.

   Pool Variants

      24hr - uses last 24hour Actual API too request profit
         -Low switching rate
      plus - uses advanced calculations to maximize profit
         -Best switching rate
      normal - uses current estimate API too request profit
         -High switching rate

  Plus Pools

      Uses calculations based on 24hr actual and current estimate prices to get more realistic estimate.
      Includes some trust index based on past 1hr currentestimate variation from 24hr.
      AND is NOT sensible to spikes.
      This shows less switching than following current estimate and more switching that following the 24hr Actual.
      Better profitability.

   Console Display Options

      Use -UIStyle Light or -UIStyle Full in config.json
            Full = Usual display
            Light = Show only currently mining info (Default)
      UIStyle automaticaly swtiches to Full during benchmarking.

   In Session Console Display Toggle

      Press key s in the window to switch between light and full display
      Press key e in the window to show/hide earnings 
      Will toggle display at next refresh

   New Version Notification

      NPlusMiner will notify new version availability

***
Copyright © 2018 MrPlus and Tesla74


![alt text](https://github.com/MrPlusGH/NPlusMiner/blob/2.1/NPM.png)
# Overclocking
!Use OC with caution!

If overclocking, the overclocking settings should be set before first run of NPlusMiner because of algorithm benchmarking.  If overclocking settings were changed after the benchmarking, you'll need to run `ResetBenchmark.bat`.

Gigabyte Xtreme Gaming Engine (VGA - XTREME ENGINE) is recommended for overclocking software.  In settings, there is a "Synchronize settings for similar graphics processors" option.
Note that it minimizes to the system tray.  To open, right click on the icon and select open.

VGA - XTREME ENGINE download:  https://www.gigabyte.com/Support/Utility/Graphics-Card

Recommended overclock settings for GeForce GTX 10 Series (1050 - 1080 Ti)
```
Power:  70% - 80% (-30 - -20)
Core:   0 - +50
Memory: +400 - +600
```

If a GPU is overclocked too high, there is a risk of crashing, freezing, and increase of bad shares.

For advanced overclocking, one can run algorithm specific overclocking by using NPlusMiner's Prerun feature and NvidiaInspector.  Make sure there isn't other overclocking software running.  Simply create a file named `<AlgoName>.bat` in the prerun folder.  If `<AlgoName>.bat` does not exist, NPlusMiner will try to launch `prerun/default.bat`.  There is a `default-Example.bat` file in the prerun folder that has example code in it.

```
Use case example 1:
Your Rig is showing issues with only one algorithm (say x16r) and you realize
it needs different OC settings than others.
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

***
Copyright © 2018 Tesla74


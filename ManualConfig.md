![alt text](https://github.com/MrPlusGH/NPlusMiner/blob/2.1/NPM.png)
# Manual configuration (Advanced)

In some scenarios, users might want to deal with configuration manually in .\config\config.json. This can be achieved by setting ManualConfig to true in this file.
Note that once set
 - NPlusMiner will not update config through the GUI anymore, all configuration has to be done manually in files.
 - AutoUpdates will not update NPlusMiner, new version will have to be installed manually.
 

## Example scenarios

1 - Need to set a specific GPU conbination

        Switch ManualConfig to true and set SelGPUCC and SelGPUDSTM to the approriate value.
        i.e. Disable GPU 4 => SelGPUCC = "0,1,2,3,5,6" and SelGPUDSTM = "0 1 2 3 5 6"

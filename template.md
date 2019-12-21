![alt text](https://github.com/MrPlusGH/NPlusMiner/blob/2.1/NPM.png)
# Using Miner Custom Configuration(advance)
*This is located at the bottom of the Configuration tab*
 all changes to configuration are refferred to as rules 
 Rules can be endabled/disabled individually after being added to the NPlus software 
- ***Algorithm*** is not pool dependant and can apply a specific code across any pool using selected algorithm
 - ***Pool*** is where you can select what pool the new rule applys to. This box can be left empty for globally applying to all selected pools.
 - ***Miner*** Defines the specific miner you want to use custom command additions on such as  defining  threads to use or other strings the miner supports **[Note:  please see individual miner program github or dev page to find supported commands]**
- ***Coin***,***Include Coins***,***Exclude Coins***  Coin can be used to include or exclude a coin from being mined on pools that support coin selection.
 - ***Custom Password additions*** is where you can apply specific code to a pool using their supported additional string `(d=X,sd=X, also currency selection c=X)`
- ***Custom Command Additions*** is where  you insert the miners supported code strings for additional commands such as gpu min and max temperature, threads to use ETC **[Note:  please see individual miner program github or dev page to find supported commands]**


**These can be used in any combination with the only Mandatory field being Algorithm.  Leaving a box blank reverts that section to the softwares predefined default. By using multiple boxes we can define things such as** : ``` pool x can mine coin y  using x threads  at z difficulty.```
 
 
***
Copyright © 2019 Designer91


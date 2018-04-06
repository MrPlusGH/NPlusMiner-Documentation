![alt text](https://github.com/MrPlusGH/NPlusMiner/blob/2.1/NPM.png)
# Autostart
To autostart the miners when starting NPlusMiner, check Autostart in the Config tab and then click on the Save Config button.

This can be done manually by editing the config.json file located in the Config folder.  Change "Autostart":  false, to "Autostart":  true,

Next open Windows Explorer and click on Folder Options.  Click on the View tab.  Check "Display the full path in the title bar" and then select "Show hidden files, folders, and drives".  Next click the OK button.

Browse to the NPlusMiner-2.x folder and right click on NPlusMiner-ConsoleUp.  Select Copy.  Next browse to `C:\Users\<user_name>\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup` and paste the NPlusMiner-ConsoleUp shortcut into the Startup folder.  Next right click on the NPlusMiner-ConsoleUp shortcut and select Properties.  Edit the target and change `".\NPlusMiner-v2.x.ps1"` to `"C:\Users\<user_name>\Desktop\NPlusMiner-v2.x\NPlusMiner-v2.x.ps1"`

Now NPlusMiner should start on Windows startup.

***
Copyright © 2018 Tesla74


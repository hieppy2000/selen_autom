* Configure Selenium Remote Grid for window
  1.  Install and configure SSH
  2.  Make sure Selenium Remote Grid jar in .bat file:
      - Create start_grid.bat file contain:
        java –jar selenium-server-standalone-2.43.1.jar -Dwebdriver C:\\chromedriver.exe
  3.  Make "start_grid.bat" file started in auto boot:
      - Create a shortcut to the batch file or "start_grid.bat"
      - Once the shortcut has been created, right-click the file and select Cut.
      - Press the Start button and type Run and press enter.
      - In the Run window, type "shell:startup" to open the Startup folder.
      - Once the Startup folder has been opened, click the Home tab at the top of the folder and select Paste to paste 
        the shortcut into the folder.
  4.  Create auto login:
      - From Start, type "RUN"
      - Enter "netplwiz", then select a user, and uncheck "User must enter username and password..."
      - Click apply and reboot window VM
  5.  Setup resolution display:
      - From Vsphere webclient or Vsphere Client GUI, select a window VM
      - Power off selected VM
      - Right click on selected VM, and launch "Edit Settings"
      - Under "Virtual Hardware" tab, select "Video Card"
      - Click on "Video Memory Caculater" and change resolution to "1920x1200"
      - Click Apply
      - Power on the VM
      - Login to window VM, and change the display setting to "1920x1200"
   6. Notes: 
      - If remote desktop to VM, it will take the RDP resolution instead of default resolution, so you need to reboot 
        the VM  to get default resolution setting in order Selenium Grid to pick up default resolution
      - Need to configure higher resolution 1600x1200 in remote desktop client so remote VM can have this high 
        resolution settings
  

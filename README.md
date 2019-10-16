# Kaiterra-Laser-Egg

Kaiterra Laser Egg v1.2 Crestron Integration Module

This module is designed to collect data from a Kaiterra Laser Egg indoor air quality monitor.  It has been tested with the Laser Egg+ Chemical monitor and the Laser Egg+ CO2 monitor.

The Laser Egg must be connected to the Kaiterra smart phone app for this code to operate.  The first step is to obtain the UUID of the monitor.  In the Kaiterra app select the device you want to obtain data from.  Then press the gear button in the upper right corner of the app to select the device settings.  Next press the information button in the upper right corner of the app.  The devices UUID is then displayed and the app provides the ability to copy it to the clipboard so it can be entered as a parameter on the Laser Egg Crestron Module.  

Next you will need to establish an account at https://dashboard.kaiterra.cn.  Once you have activated the account you can add your device to the account by entering the UUID obtained from the app.  

Finally you need to obtain a developer key.  In the upper right corner of the dashboard webpage press the gear button and select profile from the drop down menu.  From the profile options select “Developer”.   Press the “Generate a new key” button, copy the key, and enter it as a parameter on the Laser Egg Crestron module.

It should also be noted that Kaiterra provides a link on this developer page to their API documentation.

Once initialized the module will request new data from the Kaiterra IAQ monitor every 30 minutes.


# Pisces
This image is from Inigoflores
https://github.com/inigoflores/pisces-p100-tools/tree/main/SD_Image

I scaled it down with Pishrink. Now it is possible to use smaller SD cards.
I tested it with a Sandisk Max endurance 32Gb without any problems. 
It should also work with a 16 GB card. But I haven't tested it yet.

If the dashboard can be reached via the internal IP 
I have carried out the following steps to bring the miner up to date.

Select the version in the dashboard (V1-V2)
Docker miner Aktualisieren (SSH)
sudo wget http://pisces-firmware.sidcloud.cn/latest/EU/update.sh -O - | sudo bash

Sync stop (SSH)
sudo wget https://raw.githubusercontent.com/gompydo/PiscesDisableChainSync/main/apply.sh -O - | sudo bash

Dashboard version update from 0.2.8 to 0.2.9 (SSH)
sudo wget https://raw.githubusercontent.com/briffy/PiscesQoLDashboard/main/update.sh -O - | sudo bash

Then run this command to get the dashboard cached values refreshed (SSH)
sudo wget https://raw.githubusercontent.com/lt-columbo/pisces_tools/main/refresh_dashboard/refresh-dash.sh -O - | sudo bash
dd

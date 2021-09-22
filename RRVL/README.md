# retroroller-tweaks
Custom files for tweaking RRVL

In order to have latest RRVL build with latest packages, you need to do some extra work.

sudo xbps-install nano

**Repository adding**
sudo nano /etc/xbps.d/10-chaotic.conf <br>
repository=https://rrvl.chaoticneutral.eu/rrvl

**Stock dead Repository removing** <br>
sudo rm /etc/xbps.d/20-rrvl.conf

**Updates installation** <br>
sudo xbps-install -Su <br>
sudo xbps-install -S moonlight-embedded <br>
sudo xdowngrade moonlight-embedded-2.4.11_16.aarch64.xbps <br>
sudo reboot <br>

# retroroller-tweaks
Custom files for tweaking RRVL

In order to have latest RRVL build with latest packages, you need to do some extra work.

sudo xbps-install nano

**Repository adding**
sudo nano /etc/xbps.d/10-chaotic.conf
repository=https://rrvl.chaoticneutral.eu/rrvl

**Stock dead Repository removing**
sudo rm /etc/xbps.d/20-rrvl.conf

**Updates installation**
sudo xbps-install -Su
sudo xbps-install -S moonlight-embedded
sudo xdowngrade moonlight-embedded-2.4.11_16.aarch64.xbps
sudo reboot

# Eth2.0-Staking-Instructions-Installation
step-by-step guide to staking on the new Beaconchain via Raspberry Pi 4 with SSD Samsung T5 mount

Ubuntu installation guide for ssd drive (samsung T5 500gb) and boot sd card

Alternative Installation via Bootberry

1. 

1.access image from ubuntu site and use etcher to flash image onto 
both the ssd drive and sd card.

2. to add remote access via ssh
 - windows: click top of bar with files and type cmd to go to terminal
 
echo>\ssh

 - a ssh file should appear in the drive. search to confirm

3. edit config. file to proper gpu and power settings at the bottom of the .txt file

over_voltage=4
arm_freq=2000
gpu_freq=600

4. installation of ubuntu (est. time 5 min)

- login: ubuntu
- password: ubuntu

create new login as any password then...

sudo apt-get update
sudo apt-get upgrade
sudo apt-get install ubuntu-gnome-desktop

sudo reboot (once installation is complete)





Troubleshooting:

SSD Drive
#if SSD drive is not rocognized or failing to mount possible solution includes reformatting with the following format
Mac: isk utility--->select disk--->erase----exFAT----GUID Partition Map

Windows:....













blkid | grep sda1
/dev/sda1: LABEL="Samsung_T5" UUID="26B6-F73B" TYPE="exfat" PARTUUID="d33d8f5e-01"

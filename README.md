# 3D Printer Firmware for my print lab

##Klipper Configs
-Shared config files are stored in /Klipper-Config
-Machine-specific configs are stored in their own directories

### Hostname

Set the hostname of your printers' pi in `sudo raspi-config`. This hostname will be used to hardlink the correct files. Your current hostname can be seen by `echo ${HOSTNAME}`.

### Installing

To start from scratch on a new Klipper install:

```text
git clone git@github.com:will-o-matic/3DPrinterFirmware.git
cd 3DPrinterFirmware

# optionally checkout a branch
git checkout master

# install the files. 
./install.sh
```

### Uploading calibration settings etc back to github

You'll have to log into your github.

```text
cd ~/3DPrinterFirmware
./upload.sh
```

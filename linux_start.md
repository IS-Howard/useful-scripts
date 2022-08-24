# Linux_initial
Initial setting, install and useful shell script for debian base linux

## package update
```Shell
sudo apt update
sudo apt upgrade
```

## install

* Install/Upgrade the newest package
```Shell
sudo apt-get install ~
```
* Update app package list and install
```Shell
sudo apt-get update
sudo apt-get upgrade
```

* remove
```Shell
sudo apt-get remove ~
sudo apt-get purge ~   #remove setting
sudo apt autoremove    #remove dependency
sudo apt clean         #remove package files (.deb)
```

* apps
```Shell
sudo apt install vlc gimp gparted synaptic
sudo apt install ubuntu-restricted-extras
sudo apt install timeshift
sudo apt install preload
sudo apt install dkms
sudo apt install git
```

* chrome
```Shell
wget -c https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb
sudo apt-get install (-f)
```

## certain file's operation

* deb
```Shell
sudo dpkg -i *.deb
```

* sh
```Shell
sudo chmod a+x *.sh
```
```Shell
bash ./*.sh
```

* tgz
```Shell
tar -xvzf *.tgz
```

## Useful

* list detail file
```Shell
ls -l
```



# linuxconf
Useful Linux Configurations

Move launcher to the bottom:
```
gsettings set com.canonical.Unity.Launcher launcher-position Bottom
```
.bashrc alias for complete update:
```
alias update='sudo apt-get update -y && sudo apt-get upgrade -y && sudo apt-get dist-upgrade -y && sudo apt-get autoremove -y'
```

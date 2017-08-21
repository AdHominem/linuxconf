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
Read and execute updated .bashrc:
```
source ~/.bashrc
```
Compress the size of a PDF:
```
gs -sDEVICE=pdfwrite -dCompatibilityLevel=1.4 -dPDFSETTINGS=/printer -dNOPAUSE -dQUIET -dBATCH -sOutputFile=cv.pdf CVNotenspiegel.pdf
```
where `-dPDFSETTINGS` determines the quality.

.bashrc alias for downloading an entire website:
```
alias download='wget --limit-rate=200k --recursive --no-clobber --page-requisites --html-extension --convert-links --no-parent --random-wait -e robots=off -U mozilla'
```

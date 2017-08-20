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

Download an entire website:
```
wget --recursive --no-clobber --page-requisites --html-extension --convert-links --restrict-file-names=windows --domains website.org --no-parent www.website.org
```

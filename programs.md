This repo will take you through the installation process for programs and languages. The text will be based on ChromeOS boot with Linux turned on.

## Installing Software/Languages
### Verify Python Installation
- Verify Python Installation
``` Bash
~$ python --version
Python 3.9.5
```
``` Bash
~$ sudo apt install python
```

### Update pip
``` bash
python3 -m pip install --user --upgrade pip
```

### Flatpak 
- [Instructions](https://flatpak.org/setup/Chrome%20OS/)

``` Bash
 ~$ sudo apt install flatpak
 ~$ flatpak --user remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
 
### Install IDE: [VS Code](https://code.visualstudio.com/docs/setup/setup-overview) on Mac, Windows, Linux
### Install [nodejs](curl -sl https://deb.nodesource.com/setup_10.x | sudo -E bash - sudo apt-get instll -y nodejs)
### [Firefox](https://support.mozilla.org/en-US/kb/run-firefox-chromeos)
``` Bash
~$ flatpak install firefox
~$ flatpak run org.mozilla.firefox
```
### Krita
``` Bash
~$ flatpak --user install flathub org.kde.krita
~$ flatpak --user remote-add --if-not-exists kdeapps --from https://distribute.kde.org/kdeapps.flatpakrepo
```

### Pip
- Install pip on the system
``` bash
~$ sudo apt install python3-pip
```
#### Pip Packages
- [Tkinter](https://tkdocs.com/tutorial/install.html)
``` bash
~$ sudo apt-get install python3-tk 
```

- [PyQt](https://riverbankcomputing.com/)
``` bash
~$ sudo apt-get install python3-pyqt5
```

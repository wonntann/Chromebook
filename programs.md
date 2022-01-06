This repo will take you through the installation process for common programs and languages. The text will be based on ChromeOS boot with Linux turned on.

# Languages
## Install [nodejs](https://nodejs.org/en/)
 ``` bash
 sudo apt-get install nodejs```
 ```
 ``` bash
 sudo apt-get install npm
 ```

## Verify Python Installation
- Verify Python Installation
``` Bash
~$ python3 --version
Python 3.9.5
```
``` Bash
~$ sudo apt install python3
```

## Install pip
- [pip offical docs](https://packaging.python.org/en/latest/tutorials/installing-packages/)
- Enter into the terminal:
 ``` bash
 sudo apt-get install python3-pip
 ```

### Update pip
``` bash
python3 -m pip install --user --upgrade pip
```

# Flatpak 
- [Instructions](https://flatpak.org/setup/Chrome%20OS/)
- Warning: Always be vigilant of the sources and the content that you are downloading and plan to install.

``` Bash
 ~$ sudo apt install flatpak
 ~$ flatpak --user remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
 
## Install IDE: [VS Code](https://code.visualstudio.com/docs/setup/setup-overview) on Mac, Windows, Linux
-Install through flatpak, search for VS Code by entering the following command into the terminal:
  ``` bash
  flatpak search code
  ```
 - Enter the following command into the termainal from the found results, if you didn't get a search result, add the remote from [flatpak Instructions](#flatpak) or enter the following:
   ``` bash
   flatpak install flathub om.visualstudio.code 
   ```


## Firefox
- Firefox can be downloaded here [Firefox](https://support.mozilla.org/en-US/kb/run-firefox-chromeos) or you can use flatpak
``` Bash
~$ flatpak install firefox
~$ flatpak run org.mozilla.firefox
```
## Krita
``` Bash
~$ flatpak --user install flathub org.kde.krita
~$ flatpak --user remote-add --if-not-exists kdeapps --from https://distribute.kde.org/kdeapps.flatpakrepo
```
# PyQt
- [PyQt Documentation](https://riverbankcomputing.com/)
``` bash
~$ sudo apt-get install python3-pyqt5
```

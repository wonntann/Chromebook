# Chromebook


<!--  SHIELDS  -->
![GitHub](https://img.shields.io/github/license/wonntann/Chromebook?color=informational&logoColor=yellow&style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/wonntann/Chromebook?color=red&style=for-the-badge)
![GitHub Issues](https://img.shields.io/github/issues-raw/wonntann/Chromebook?color=critical&style=for-the-badge)
![Twitter](https://img.shields.io/twitter/follow/wonntann?color=red&style=for-the-badge)


<!--  PROJECT INTRO  -->
<br />
<div align="center">Notes on working on a Chromebook, install crouton/dual boot xfce or work with enable Linux and work within Chromebook boot</div>

# How To Read
- If you would like to jump to sections, locate the **Table of Contents** menu in the upper left of this repo GitHub header and select from the dropdown
- Using Linux, you can use chroot dualboot or enable Linux on your Chromebook, either way it is personal preference.



<!--  ABOUT PROJECT  -->
## About The Project
This repo will contain Chromebook notes that you can fork and work with. I will try to add more notes throughout the month. If you find any errors or would like to contribute, please look at the Contributing.md.
<p align="right">(<a href="#top">back to top</a>)</p>

## Built With
``` Bash
~$ cat /etc/os-release
PRETTY_NAME="Debian GNU/Linux 10 (buster)"
NAME="Debian GNU/Linux"
VERSION_ID="10"
VERSION="10 (buster)"
VERSION_CODENAME=buster
ID=debian
HOME_URL="https://www.debian.org/"
SUPPORT_URL="https://www.debian.org/support"
BUG_REPORT_URL="https://bugs.debian.org/"
```
<p align="right">(<a href="#top">back to top</a>)</p>


## Getting Started
There are two options for running Linux on your Chromebook. Option #1: Enabling Linux and using on the ChromOS boot or Option#2: Dualboot through the chroot installation.
Option #1:
- Open Chromebook
- Enable Linux
- Install needed packages

Option #1:
- Open Chromebook
- Enter Developer/Recovery Mode
- Download and install crouton
- Start to dual boot

# Installation
## Linux on ChromeOS
- [Enable Linux](https://support.google.com/chromebook/answer/9145439)
1. Open Chrome and enter **chrome://os-settings** into the address bar
2. Navigate to the menu options, open **Advanced** --> **Developers** --> Select the **Turn On** Linux option (It will take a few moments to activate, when done the Linux terminal will be accessible and found in the ChromeOS apps menu page.)


## Linux with chroot
- Boot Chromebook and enter Developer/Recovery Mode by pressing **Esc + Refresh + Power** buttons
- In Recovery mode, press **Ctrl + d** and hit **Enter** on "Turn OS Verification Off" prompt
  - You will need to press **Ctrl + d** everytime you reboot
- Press **Ctrl + Alt + t** to open Shell (If not open, run Chrome and press **Ctrl + Alt + t** 
- Download [Crouton](https://andauth.co/EI1nA6(
- Type **Shell**
- Type  
    ``` bash 
    ~$ sudo install -Dt /usr/local/bin -m 755 ~/Downloads/crouton
    ```
    and confirm with the Enter key.
- Run installer
  ``` bash
  ~$ sudo crouton -t xfce
  ```
- ...Sometime later...run  Xfce session
  ``` bash
  ~$ sudo enter-chroot startxfce4
  ```

### Dual boot Linux with chroot
- Press **Ctrl + d** at OS Verification screen
- Press **Ctrl + Alt + t** to open crosh and type:
  ``` bash
  ~$ sudo enter-chroot startxfce4
  ```
- Cycle through Chromium OS and your graphical chroots by typing **Ctrl + Alt + Shift + Back** or **Ctrl + Alt + Shift + Forward** 

***See GitHub repo at [crouton](https://github.com/dnschneid/crouton)

## Installing Software/Languages
### Verify Python Installation
- Verify Python Installation
``` Bash
~$ python--version
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


## Troubleshooting
### ChromeOS with Linux Turned On
This will be addressing issues on ChromeOS Linux, but you can apply some of them to either boot. Follow each point in order or jump to the bullet point that you need to address your issues.

* Restart ChromeOS
* Update packages through the Terminal app, run this command:
  ``` bash
  sudo apt-get update && sudo apt-get dist-upgrade
  ``` 
* Open termina in Chrome browser by entering:
  ``` bash
  vsh termina
  ```
* To create a gnu-container, enter the termina, then type the following command:
* ``` bash
  lxc config set penguin security.nesting true
  lxc launch ubuntu:18.04
   ```
 
  
## Resources
- [Learn Python Reddit](https://www.reddit.com/r/learnpython/)
- [Keyboard Shortcuts](https://support.google.com/chromebook/answer/183101?hl=en)


## Keyboard Shortcuts
- Page up/down                              Alt + Up/Down arrow
- Top/Bottom of page                        Ctrl + Alt + Up/Down arrow
- Stop the loading of your current page     Esc
- View page source                          Ctrl + u
- Show or hide the Developer Tools panel    Shift + Ctrl + i
- Turn Caps Lock on or off                  Search + Alt (or) Launcher  + Alt
- Move to beginning/end of the line         Search + Left/Right arrow or Launcher + L/R arrow 
- Delete previous word                      Ctrl + Backspace




## Contributing
Thanks for checking out this repo, hopefully it will/has assisted you. If you found any edits or want to contribute, please do, it might assist someone who was struggling with this subject.

Submit an issue or I encourage you to fork this repo and contribute to this project!

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b my-edits)
3. Commit your Changes (`git commit -m 'Add some new edits to <documentation> for <what it does>'`)
4. Push to the Branch (`git push origin new edits`)
5. Open a Pull Request


## License

Distributed under the MIT License. See [License](https://github.com/wonntann/Chromebook/blob/main/LICENSE) for more information.



## Contact
Tanya - [@wonntann](https://twitter.com/wonntann)

Project Link: [https://github.com/wonntann/gitHub](https://github.com/wonntann/gitHub)

<p align="right">(<a href="#top">back to top</a>)</p>



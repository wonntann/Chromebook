# Chromebook


<!--  SHIELDS  -->
![GitHub](https://img.shields.io/github/license/wonntann/Chromebook?color=informational&logoColor=yellow&style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/wonntann/Chromebook?color=red&style=for-the-badge)
![GitHub Issues](https://img.shields.io/github/issues-raw/wonntann/Chromebook?color=critical&style=for-the-badge)
![Twitter](https://img.shields.io/twitter/follow/wonntann?color=red&style=for-the-badge)


<!--  PROJECT INTRO  -->
<br />
<div align="center">Notes on working on a Chromebook</div>


<!--  TABLE OF CONTENTS  -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#getting-started">Getting Started</a></li>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#programs">Programs</a></li>
      </ul>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#resources">Resources</a></li>
    <li><a href="#keyboard-shortcuts">Keyboard Shortcuts</a></li>
  </ol>
</details>


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
- Open Chromebook
- Enable Linux
- Install needed packages
<p align="right">(<a href="#top">back to top</a>)</p>


## Prerequisite
- [Enable Linux](https://support.google.com/chromebook/answer/9145439)
<p align="right">(<a href="#top">back to top</a>)</p>


## Installation
- Install IDE: [VS Code](https://code.visualstudio.com/docs/setup/setup-overview) on Mac, Windows, Linux
- Install [nodejs](curl -sl https://deb.nodesource.com/setup_10.x | sudo -E bash - sudo apt-get instll -y nodejs)


### Verify Installation
- Verify Python Installation
``` Bash
~$ python--version
Python 3.9.5
```
``` Bash
~$ sudo apt install python
```

### Flatpak 
- [Instructions](https://flatpak.org/setup/Chrome%20OS/)

``` Bash
 ~$ sudo apt install flatpak
 ~$ flatpak --user remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

### Programs 
- [Firefox](https://support.mozilla.org/en-US/kb/run-firefox-chromeos)
``` Bash
~$ flatpak install firefox
~$ flatpak run org.mozilla.firefox
```
- Krita
``` Bash
~$ flatpak --user install flathub org.kde.krita
~$ flatpak --user remote-add --if-not-exists kdeapps --from https://distribute.kde.org/kdeapps.flatpakrepo
```

<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing
Thanks for checking out this page, since the more positive edits and critics of this repo will help this project benefit more individuals.

Submit an issue or I encourage you to fork this repo and make another page in the changes directory and contribute to this project!

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>


## License

Distributed under the MIT License. See [License](https://github.com/wonntann/Python_Projects/blob/main/LICENSE) for more information.
<p align="right">(<a href="#top">back to top</a>)</p>


## Contact
Tanya - [@wonntann](https://twitter.com/wonntann)

Project Link: [https://github.com/wonntann/gitHub](https://github.com/wonntann/gitHub)

<p align="right">(<a href="#top">back to top</a>)</p>


## Resources
- [Learn Python Reddit](https://www.reddit.com/r/learnpython/)
- [Keyboard Shortcuts](https://support.google.com/chromebook/answer/183101?hl=en)

<p align="right">(<a href="#top">back to top</a>)</p>

## Keyboard Shortcuts
- Page up/down                              Alt + Up/Down arrow
- Top/Bottom of page                        Ctrl + Alt + Up/Down arrow
- Stop the loading of your current page     Esc
- View page source                          Ctrl + u
- Show or hide the Developer Tools panel    Shift + Ctrl + i
- Turn Caps Lock on or off                  Search + Alt (or) Launcher  + Alt
- Move to beginning/end of the line         Search + Left/Right arrow or Launcher + L/R arrow 
- Delete previous word                      Ctrl + Backspace


<p align="right">(<a href="#top">back to top</a>)</p>

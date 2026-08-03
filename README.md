<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/AfroPK/borderless-fullscreen">
    <img src="icon-bf.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Borderless Fullscreen</h3>

  <p align="center">
    A shell script that forces a selected windowed application into borderless fullscreen mode on Linux. Inspired by Borderless Gaming for Windows.
    <br />
    <a href="https://github.com/AfroPK/borderless-fullscreen"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/AfroPK/borderless-fullscreen">View Demo</a>
    &middot;
    <a href="https://github.com/AfroPK/borderless-fullscreen/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/AfroPK/borderless-fullscreen/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

**Borderless Fullscreen** is a shell script that lets you force a selected windowed application into borderless fullscreen mode on Linux. It works on both **Xorg** and **Wayland** and is inspired by the [Borderless Gaming](https://github.com/Codeusa/Borderless-Gaming) app for Windows.

* Perfect for games and apps that don't natively support windowed-borderless mode
* Works on Xorg & Wayland
* Simple installer that adds it to your application menu

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

[![Shell][Shell]][Shell-url]
* [![Xdotool](https://img.shields.io/badge/Xdotool-362D59?style=for-the-badge&logo=linux&logoColor=white)][xdotool-url]
* [![wlr-randr](https://img.shields.io/badge/wlr--randr-362D59?style=for-the-badge&logo=linux&logoColor=white)][wlr-url]
* [![zenity](https://img.shields.io/badge/Zenity-362D59?style=for-the-badge&logo=linux&logoColor=white)][zenity-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

Requirements differ by display server.

**Xorg**
* xdotool
* wmctrl
* zenity

**Wayland**
* wlr-randr
* wmctrl
* zenity

### Installation

1. Install the required dependencies for your display server and distro.

**Debian / Ubuntu**
```sh
# Xorg
sudo apt-get install xdotool zenity
# Wayland
sudo apt-get install wlr-randr wmctrl zenity
```

**Fedora**
```sh
# Xorg
sudo dnf install xdotool zenity
# Wayland
sudo dnf install wlr-randr wmctrl zenity
```

**Arch**
```sh
sudo pacman -Syu xdotool zenity
```

**Alpine**
```sh
apk add --upgrade xdotool zenity
```

2. Clone the repo and install.
```sh
git clone https://github.com/AfroPK/borderless-fullscreen.git
cd borderless-fullscreen
sudo chmod +x install.sh
sudo ./install.sh
```
3. Choose **Wayland** or **Xorg** when prompted.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

After installing, **Borderless Fullscreen** will appear in your application menu. Launch it and select the window you want to force into borderless fullscreen.

To remove it:
```sh
sudo ./uninstall.sh
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [ ] Add more features
- [ ] Improve documentation

See the [open issues](https://github.com/AfroPK/borderless-fullscreen/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- LICENSE -->
## License

Distributed under the GPL-3.0 License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

AfroPK - [@AfroPK](https://github.com/AfroPK)

Project Link: [https://github.com/AfroPK/borderless-fullscreen](https://github.com/AfroPK/borderless-fullscreen)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
* [Img Shields](https://shields.io/)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/AfroPK/borderless-fullscreen.svg?style=for-the-badge
[contributors-url]: https://github.com/AfroPK/borderless-fullscreen/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/AfroPK/borderless-fullscreen.svg?style=for-the-badge
[forks-url]: https://github.com/AfroPK/borderless-fullscreen/network/members
[stars-shield]: https://img.shields.io/github/stars/AfroPK/borderless-fullscreen.svg?style=for-the-badge
[stars-url]: https://github.com/AfroPK/borderless-fullscreen/stargazers
[issues-shield]: https://img.shields.io/github/issues/AfroPK/borderless-fullscreen.svg?style=for-the-badge
[issues-url]: https://github.com/AfroPK/borderless-fullscreen/issues
[license-shield]: https://img.shields.io/github/license/AfroPK/borderless-fullscreen.svg?style=for-the-badge
[license-url]: https://github.com/AfroPK/borderless-fullscreen/blob/master/LICENSE.txt
[Shell]: https://img.shields.io/badge/Shell-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white
[Shell-url]: https://www.gnu.org/software/bash/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[node-url]: https://nodejs.org/
[express-url]: https://expressjs.com/
[vite-url]: https://vitejs.dev/
[xdotool-url]: https://github.com/jordansissel/xdotool
[wlr-url]: https://sr.ht/~emersion/wlr-randr/
[zenity-url]: https://wiki.gnome.org/Projects/Zenity
[python-url]: https://www.python.org/
[pyqt-url]: https://www.riverbankcomputing.com/software/pyqt/

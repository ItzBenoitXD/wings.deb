<br/>
<p align="center">
  <a href="https://github.com/ItzBenoitXD/wings.deb">
    <img src="https://miro.medium.com/v2/resize:fit:364/0*6JLUUwz_R66XlSjk.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">wings.deb</h3>

  <p align="center">
    The server control plane for Pterodactyl Panel, packaged by a .deb
    <br/>
    <br/>
    <a href="https://github.com/ItzBenoitXD/wings.deb"><strong>Explore the docs »</strong></a>
    <br/>
    <br/>
    <a href="https://github.com/ItzBenoitXD/wings.deb">View Demo</a>
    .
    <a href="https://github.com/ItzBenoitXD/wings.deb/issues">Report Bug</a>
    .
    <a href="https://github.com/ItzBenoitXD/wings.deb/issues">Request Feature</a>
  </p>
</p>

![Downloads](https://img.shields.io/github/downloads/ItzBenoitXD/wings.deb/total) ![Contributors](https://img.shields.io/github/contributors/ItzBenoitXD/wings.deb?color=dark-green) ![Forks](https://img.shields.io/github/forks/ItzBenoitXD/wings.deb?style=social) ![Stargazers](https://img.shields.io/github/stars/ItzBenoitXD/wings.deb?style=social) ![Issues](https://img.shields.io/github/issues/ItzBenoitXD/wings.deb) ![License](https://img.shields.io/github/license/ItzBenoitXD/wings.deb) 

## Table Of Contents

* [About the Project](#about-the-project)
* [Built With](#built-with)
* [Getting Started](#getting-started)
  * [Prerequisites](#prerequisites)
  * [Installation](#installation)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [License](#license)
* [Authors](#authors)
* [Acknowledgements](#acknowledgements)

## About The Project

I had no idea on what to do on GitHub, so I made this. 
Wings is Pterodactyl's server control plane, built for the rapidly changing gaming industry and designed to be highly performant and secure. Wings provides an HTTP API allowing you to interface directly with running server instances, fetch server logs, generate backups, and control all aspects of the server lifecycle.

In addition, Wings ships with a built-in SFTP server allowing your system to remain free of Pterodactyl specific dependencies, and allowing users to authenticate with the same credentials they would normally use to access the Panel. (copied straight from https://github.com/pterodactyl/wings)

## Built With

* dpkg (for the package)
* Go (for Wings itself)

## Getting Started

Getting started is pretty easy so I'll explain in a little bit of steps.

### Prerequisites

To install this package, you will need:

* A package manager that can install .deb files

* Docker

```sh
curl -sSL https://get.docker.com/ | CHANNEL=stable bash
sudo systemctl enable --now docker
```

* that's all? i don't know

### Installation

There are only 3 commands you need to run to install Wings.
```sh
sudo mkdir -p /etc/pterodactyl
curl -L -o ~/wings_linux.deb "https://github.com/ItzBenoitXD/wings.deb/releases/latest/download/wings-linux-$([[ "$(uname -m)" == "x86_64" ]] && echo "amd64" || echo "arm64").deb"
sudo apt-get install -f ~/wings_linux.deb
```

## Roadmap

See the [open issues](https://github.com/ItzBenoitXD/wings.deb/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.
* If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/ItzBenoitXD/wings.deb/issues/new) to discuss it, or directly create a pull request after you edit the *README.md* file with necessary changes.
* Please make sure you check your spelling and grammar.
* Create individual PR for each suggestion.
* Please also read through the [Code Of Conduct](https://github.com/ItzBenoitXD/wings.deb/blob/main/CODE_OF_CONDUCT.md) before posting your first idea as well.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See [LICENSE](https://github.com/ItzBenoitXD/wings.deb/blob/main/LICENSE.md) for more information.

## Authors

* **Shaan Khan** - *Comp Sci Student* - [Shaan Khan](https://github.com/ShaanCoding/) - *Built ReadME Template*
* **Matthew Penner and the entire Pterodactyl Team** - *Open-source game server management panel* - [Matthew Penner and the entire Pterodactyl Team](https://github.com/pterodactyl) - *Helped make this project possible*
* **ItzBenoitXD** - *random guy* - [ItzBenoitXD](https://github.com/ItzBenoitXD) - *Made this project*

## Acknowledgements

* [ShaanCoding](https://github.com/ShaanCoding/)
* [Othneil Drew](https://github.com/othneildrew/Best-README-Template)
* [ImgShields](https://shields.io/)
* [Pterodactyl](https://github.com/pterodactyl)

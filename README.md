[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/capcodigital/devops-maturity">
    <img src="https://raw.githubusercontent.com/capcodigital/.github/master/images/capco.jpeg" alt="Logo" height="160px">
  </a>
  <h3 align="center">DevOps Maturity - Best Practice Guidelines</h3>
  <p align="center">
    The purpose of this repository is to provide DevOps Best Practice Guidelines which can be referenced from Capco's DevOps Maturity Assessment dashboard.
    <br />
    <a href="https://github.com/capcodigital/devops-maturity"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/capcodigital/devops-maturity">View Demo</a>
    ·
    <a href="https://github.com/capcodigital/devops-maturity/issues">Report Bug</a>
    ·
    <a href="https://github.com/capcodigital/devops-maturity/issues">Request Feature</a>
  </p>
</p>

<details>
  <summary>Contents</summary>
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [About The Project](#about-the-project)
- [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Local Dependencies](#local-dependencies)
  - [Local Setup](#local-setup)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
</details>

## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

The purpose of this repository is to provide DevOps Best Practice Guidelines which can be referenced from Capco's DevOps Maturity Assessment dashboard.

* [Culture](guidelines/culture/README.md)
* [Continuous Delivery](guidelines/continuous-delivery/README.md)


## Built With

Further logos should be inserted to highlight the specific technologies used to create the solution from [here](https://github.com/Ileriayo/markdown-badges).

![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

## Getting Started

To get a local copy up and running follow these simple steps.

### Local Dependencies

A number of local dependencies are required.  To review the local dependencies:

* When using MacOS run `make requirements`
* otherwise run `cat Brewfile` to inspect the requirements

If additional dependencies are required they should be added to `Brewfile`, for more details please review the official `brew bundle` documentation [here](https://github.com/Homebrew/homebrew-bundle).

### Local Setup

This repo follows the principle of minimal manual setup of the local development environment.

 A `make` target has been provided for simplicity ```make init```, the `make` file can be inspected for more details.

 ```shell
# use the folder name as the repo name
make init

# explicitly pass in the repo name (e.g. my-service)
make repo=my-service init
```

If at any point the repo name needs to be changed then the `make rename` target can be called.

```shell
make repo=my-service rename
```

## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

## Roadmap

See the [open issues](https://github.com/capcodigital/devops-maturity/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

If you would like to contribute to any Capco Digital OSS projects please read:

* [Code of Conduct](https://github.com/capcodigital/.github/blob/master/CODE_OF_CONDUCT.md)
* [Contributing Guidelines](https://github.com/capcodigital/.github/blob/master/CONTRIBUTING.md)

## License

Distributed under the MIT License. See `LICENSE` for more information.

* [Best README Template](https://github.com/othneildrew/Best-README-Template)
* [Markdown Badges](https://github.com/Ileriayo/markdown-badges)
* [DocToc](https://github.com/thlorenz/doctoc)

[contributors-shield]: https://img.shields.io/github/contributors/capcodigital/devops-maturity.svg?style=for-the-badge
[contributors-url]: https://github.com/capcodigital/devops-maturity/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/capcodigital/devops-maturity.svg?style=for-the-badge
[forks-url]: https://github.com/capcodigital/devops-maturity/network/members
[stars-shield]: https://img.shields.io/github/stars/capcodigital/devops-maturity.svg?style=for-the-badge
[stars-url]: https://github.com/capcodigital/devops-maturity/stargazers
[issues-shield]: https://img.shields.io/github/issues/capcodigital/devops-maturity.svg?style=for-the-badge
[issues-url]: https://github.com/capcodigital/devops-maturity/issues
[license-shield]: https://img.shields.io/github/license/capcodigital/devops-maturity.svg?style=for-the-badge
[license-url]: https://github.com/capcodigital/devops-maturity/blob/master/LICENSE
[product-screenshot]: images/screenshot.png

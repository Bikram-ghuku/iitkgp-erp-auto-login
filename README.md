<div id="top"></div>

<!-- PROJECT SHIELDS -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links-->
<div align="center">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Wiki][wiki-shield]][wiki-url]

</div>

<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/metakgp/iitkgp-erp-auto-login">
     <img width="140" alt="image" src="./src/assets/images/ext_icon.png">
  </a>

  <h3 align="center">ERP Auto Login - IIT KGP</h3>

<p align="Center">
  <a href="https://addons.mozilla.org/en-US/firefox/addon/erp-auto-login-iitkgp/">
    <img src="https://blog.mozilla.org/addons/files/2020/04/get-the-addon-fx-apr-2020.svg" alt="ERP Auto Login - IIT KGP logo" height="58">
  </a>
  <a href="https://chrome.google.com/webstore/detail/erp-auto-login-iitkgp/hianmedhblomknonbbmalncjjffdligl">
    <img src="https://storage.googleapis.com/web-dev-uploads/image/WlD8wC6g8khYWPJUsQceQkhXSlv1/UV4C4ybeBTsZt43U4xis.png" alt="ERP Auto Login - IIT KGP logo">
  </a>
</p>

  <p align="center">
    Minimial yet powerful and customizable autologin/autofill extension, for IIT KGP students
    <br />
    <a href="https://github.com/metakgp/iitkgp-erp-auto-login/issues">Request Feature / Report Bug</a>
  </p>
</div>


<!-- TABLE OF CONTENTS -->
<details>
<summary>Table of Contents</summary>

- [About The Project](#about-the-project)
- [Building from source](#building-from-source)
  - [Prerequisites](#prerequisites)
  - [Development](#development)
  - [Deployment](#deployment)
- [Usage](#usage)
- [Contact](#contact)
  - [Maintainer(s)](#maintainers)
  - [Creators(s)](#creators)
- [Additional documentation](#additional-documentation)

</details>


<!-- ABOUT THE PROJECT -->
## About The Project
<!-- UPDATE -->
<div align="center">
  <a href="https://github.com/metakgp/iitkgp-erp-auto-login">
    <img width="80%" alt="image" src="./screenshots/cover_new.png">
  </a>
</div>

ERP Auto Login is a browser extension supporting both chrome and firefox. The extension stores the users ERP credentials like username, password and security questions and fills them up automatically whenever the user opens the ERP. It also sends the OTP to the email, the user only need to fill up the OTP and continue to login.

<p align="right">(<a href="#top">back to top</a>)</p>

## Building from source

To set up a local instance of the application, follow the steps below.

### Prerequisites

The following dependencies are required to be installed for the project to function properly:

* npm
  ```sh
  npm install npm@latest -g
  ```
* web-ext
  ```sh
  npm install --global web-ext
  ```
* Clone the repository and move to the cloned directory
  ```bash
  git clone https://github.com/metakgp/iitkgp-erp-auto-login.git
  cd iitkgp-erp-auto-login
  ```
* Install the dependencies
  ```bash
  npm install
  ```

<p align="right">(<a href="#top">back to top</a>)</p>

### Development

  1. Build the extension and watch for changes
     ```bash
     npm run start
     ```
  2. The above step will create a `addon` folder with the extension in it.
      ```bash
      cd addon
      ```
  3. Run the extension using [web-ext](https://extensionworkshop.com/documentation/develop/getting-started-with-web-ext/) as below, this starts a new browser window with the extension, this version supports hot reload
     ```bash
     web-ext run # run the extension for firefox
     web-ext run -t chromium # (or) run the extension for chrome
     ```
<p align="right">(<a href="#top">back to top</a>)</p>

### Deployment

  1. Build the extension and watch for changes
     ```bash
     npm run build-prod
     ```
     > The above step will create a `addon` folder with the extension in it.
  3. Adding to Browser:
      - For Chrome:
        - Open new tab and type `chrome://extensions` on search bar.
        - Toggle the **DEVELOPER MODE** on top right corner.
        - Click **LOAD UNPACKED** option, browse to the cloned folder and select the [addon](./addon) folder.
    
      - For Firefox:
        - Open new tab and type `about:debugging#/runtime/this-firefox` on search bar.
        - Click on the `Load Temporary Add-on...` button under **Load Temporary Extensions** Section.
        - Navigate to [addon](./addon) folder in your opened file navigator.
        - Select the `manifest.json` file inside it and press **open**.

<p align="right">(<a href="#top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->
## Usage
Screenshots of the extension

| ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(1).png>) | ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(7).png>) | ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(2).png>) |
| -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(5).png>) | ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(4).png>) | ![](</screenshots/chrome-extension___hianmedhblomknonbbmalncjjffdligl_pages_Popup_index.html%20(3).png>) |

<p align="right">(<a href="#top">back to top</a>)</p>

## Contact

<p>
📫 Metakgp -
<a href="https://slack.metakgp.org">
  <img align="center" alt="Metakgp's slack invite" width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/slack.svg" />
</a>
<a href="mailto:metakgp@gmail.com">
  <img align="center" alt="Metakgp's email " width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/gmail.svg" />
</a>
<a href="https://www.facebook.com/metakgp">
  <img align="center" alt="metakgp's Facebook" width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/facebook.svg" />
</a>
<a href="https://www.linkedin.com/company/metakgp-org/">
  <img align="center" alt="metakgp's LinkedIn" width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/linkedin.svg" />
</a>
<a href="https://twitter.com/metakgp">
  <img align="center" alt="metakgp's Twitter " width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/twitter.svg" />
</a>
<a href="https://www.instagram.com/metakgp_/">
  <img align="center" alt="metakgp's Instagram" width="22px" src="https://raw.githubusercontent.com/edent/SuperTinyIcons/master/images/svg/instagram.svg" />
</a>
</p>

### Maintainer(s)

The currently active maintainer(s) of this project.

- [Arpit Bhardwaj](https://github.com/proffapt)

### Creator(s)

Honoring the original creator(s) and ideator(s) of this project.

<!-- UPDATE -->
- [Siddhartha Sarkar](https://github.com/siddsarkar)

<p align="right">(<a href="#top">back to top</a>)</p>

## Additional documentation

  - [License](/LICENSE)
  - [Code of Conduct](/.github/CODE_OF_CONDUCT.md)
  - [Security Policy](/.github/SECURITY.md)
  - [Contribution Guidelines](/.github/CONTRIBUTING.md)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->

[contributors-shield]: https://img.shields.io/github/contributors/metakgp/iitkgp-erp-auto-login.svg?style=for-the-badge
[contributors-url]: https://github.com/metakgp/iitkgp-erp-auto-login/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/metakgp/iitkgp-erp-auto-login.svg?style=for-the-badge
[forks-url]: https://github.com/metakgp/iitkgp-erp-auto-login/network/members
[stars-shield]: https://img.shields.io/github/stars/metakgp/iitkgp-erp-auto-login.svg?style=for-the-badge
[stars-url]: https://github.com/metakgp/iitkgp-erp-auto-login/stargazers
[issues-shield]: https://img.shields.io/github/issues/metakgp/iitkgp-erp-auto-login.svg?style=for-the-badge
[issues-url]: https://github.com/metakgp/iitkgp-erp-auto-login/issues
[license-shield]: https://img.shields.io/github/license/metakgp/iitkgp-erp-auto-login.svg?style=for-the-badge
[license-url]: https://github.com/metakgp/iitkgp-erp-auto-login/blob/master/LICENSE
[wiki-shield]: https://custom-icon-badges.demolab.com/badge/metakgp_wiki-grey?logo=metakgp_logo&style=for-the-badge
[wiki-url]: https://wiki.metakgp.org
[slack-url]: https://slack.metakgp.org
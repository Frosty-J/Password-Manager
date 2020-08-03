# Password Manager
[![Build Status](https://travis-ci.org/zeruniverse/Password-Manager.svg)](https://travis-ci.org/zeruniverse/Password-Manager)
[![Codacy Badge](https://api.codacy.com/project/badge/grade/b5d954be72144355aa258748cfd05bca)](https://www.codacy.com/app/zzy8200/Password-Manager)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/zeruniverse/Password-Manager/blob/master/LICENSE)
![Environment](https://img.shields.io/badge/PHP-7.1+-blue.svg)
![Environment](https://img.shields.io/badge/MySQL-required-ff69b4.svg)

**'master' branch is a dev-branch, please download stable version from [Release](https://github.com/zeruniverse/Password-Manager/releases) to use it.**

## Version

v11.00

Supports are available [here](https://github.com/zeruniverse/Password-Manager/issues) for versions greater than v9.13

Please note, Password-Manager only supports **HTTPS**

## DEMO
[phppasswordmanager.sourceforge.io](https://phppasswordmanager.sourceforge.io)

This demo is for test **ONLY**! Do **NOT** put your real password there.

You can access the database for this demo [here](https://mysql-p.sourceforge.net), with login username **p2663268ro** and password **12345678**

## Features

1. Client side encryption. Server only keeps the encrypted strings. **Strong encryption**: Server side uses PBKDF2+SHA3-512, client side uses AES256 / PBKDF2+[SHA512|SHA3-512]  (SHA512 is used in client side as Javascript SHA3 is too slow)  [See more about security analysis](https://github.com/zeruniverse/Password-Manager/wiki/Mechanism#safety)

2. Customized fields support. You can add and delete fields for the password manager. You might want a URL field to keep login URL for all your accounts.

3. PIN login. You don't need to input your long login password everytime. Instead, you can use a short PIN, in your trusted devices.

4. Files support. You can attach files to accounts. Of course, files are encrypted in your browser before they are uploaded.

5. Tags support and searching support. This makes it easier to manage lots of accounts.

6. Import/Export as CSV file.

7. Easy to backup and recovery.

8. Authentication control. Account/IP will be blocked for too many failed attempts. After a short time of no action, you'll sign out automatically.

9. Friendly UI.

## Installation
See [wiki](https://github.com/zeruniverse/Password-Manager/wiki/Installation)

## How to use
See [wiki](https://github.com/zeruniverse/Password-Manager/wiki)

## Web Browser Plugin

Chrome: [Chrome Web Store](https://chrome.google.com/webstore/detail/password-manager/mbfjokpccbakbnnpklkcginkalkijkan)

Firefox: [Add-on](https://addons.mozilla.org/en-US/firefox/addon/self-hosted-password-addon/)

GitHub Project: [PwChromeExtension](https://github.com/BenjaminHae/PwChromeExtension) by Benjamin.

## Mechanism

<img width="1098" alt="mechanism" src="https://cloud.githubusercontent.com/assets/4648756/13795540/b0dfde78-eabe-11e5-8407-e5904dad59d2.png">

You can read more information about implementation in [wiki](https://github.com/zeruniverse/Password-Manager/wiki/Mechanism).

## Extentions
You can easily add E-mail verification, Google authentication... in your version of password manager. Put your implementation inside `src/rest/check.php`, which is used for login authentication.

## Contribution

Please read the [guide](https://github.com/zeruniverse/Password-Manager/wiki/Contribution) first.

All contributors to this project must agree their work to be published under MIT license ONLY (see LICENSE file) before submitting a pull request.

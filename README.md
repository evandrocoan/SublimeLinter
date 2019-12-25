SublimeLinter
=============

[![Build Status](https://img.shields.io/travis/SublimeLinter/SublimeLinter/master.svg)](https://travis-ci.org/SublimeLinter/SublimeLinter)

The code linting framework for [Sublime Text 3](http://sublimetext.com/3).
No linters included: get them via [Package Control](https://packagecontrol.io/search/SublimeLinter).

<img src="https://raw.githubusercontent.com/SublimeLinter/SublimeLinter/master/docs/screenshot.png" width="848">


## Installation

### By Package Control

1. Download & Install **`Sublime Text 3`** (https://www.sublimetext.com/3)
1. Go to the menu **`Tools -> Install Package Control`**, then,
   wait few seconds until the installation finishes up
1. Now,
   Go to the menu **`Preferences -> Package Control`**
1. Type **`Add Channel`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
   input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Go to the menu **`Tools -> Command Palette...
   (Ctrl+Shift+P)`**
1. Type **`Preferences:
   Package Control Settings – User`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
   find the following setting on your **`Package Control.sublime-settings`** file:
   ```js
       "channels":
       [
           "https://packagecontrol.io/channel_v3.json",
           "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
       ],
   ```
1. And,
   change it to the following, i.e.,
   put the **`https://raw.githubusercontent...`** line as first:
   ```js
       "channels":
       [
           "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
           "https://packagecontrol.io/channel_v3.json",
       ],
   ```
   * The **`https://raw.githubusercontent...`** line must to be added before the **`https://packagecontrol.io...`** one, otherwise,
     you will not install this forked version of the package,
     but the original available on the Package Control default channel **`https://packagecontrol.io...`**
1. Now,
   go to the menu **`Preferences -> Package Control`**
1. Type **`Install Package`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
search for **`SublimeLinter`** and press <kbd>Enter</kbd>

See also:

1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## Settings

Settings are mostly documented in the [default settings](https://github.com/SublimeLinter/SublimeLinter/blob/master/SublimeLinter.sublime-settings). When you open the SublimeLinter settings you'll see them on the left.

- Additional information is in our docs at [sublimelinter.com](http://sublimelinter.com/).
- Read about all the changes between 3 and 4 [here](https://raw.githubusercontent.com/SublimeLinter/SublimeLinter/master/messages/4.0.0.txt).


## Key Bindings

SublimeLinter comes with some pre-defined keyboard shortcuts. You can customize these via the Package Settings menu.

| Command         | Linux & Windows  | MacOS                  |
|-----------------|------------------|------------------------|
| Lint this view  | CTRL + K, L      | CTRL + CMD + L         |
| Show all errors | CTRL + K, A      | CTRL + CMD + A         |
| Goto next error | CTRL + K, N      | CTRL + CMD + E         |
| Goto prev error | CTRL + K, P      | CTRL + CMD + SHIFT + E |


## Support & Bugs

Please use the [debug mode](http://www.sublimelinter.com/en/stable/troubleshooting.html#debug-mode)
and include all console output, and your settings in your
[bug report](https://github.com/SublimeLinter/SublimeLinter/issues/new).
If your issue is specific to a particular linter, please report it on that linter's repository instead.


## Creating a linter plugin

Fork the [template](https://github.com/SublimeLinter/SublimeLinter-template) to get started on your plugin.
It contains a howto with all the information you need.

---------------------------


If you use SublimeLinter and feel it is making your coding life better and easier,
please consider making a donation for all the coffee and beer involved in this project.
Thank you!

Donate via:
* [**Paypal**](https://paypal.me/pools/c/82jmBQtUbY)

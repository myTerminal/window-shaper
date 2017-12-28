# window-shaper

[![Marmalade](https://img.shields.io/badge/marmalade-available-8A2A8B.svg)](https://marmalade-repo.org/packages/window-shaper)  
[![License](https://img.shields.io/badge/LICENSE-GPL%20v3.0-blue.svg)](https://www.gnu.org/licenses/gpl.html)
[![Gratipay](http://img.shields.io/gratipay/myTerminal.svg)](https://gratipay.com/myTerminal)

A utility to easily resize windows within Emacs.

You can use window-shaper to resize windows with a press of a single key.

## Installation

### Manual

Save the file *window-shaper.el* to disk and add the directory containing it to `load-path` using a command in your *.emacs* file like:

    (add-to-list 'load-path "~/.emacs.d/")

The above line assumes that you've placed the file into the Emacs directory '.emacs.d'.

Start the package with:

    (require 'window-shaper)

### Marmalade

If you have Marmalade added as a repository to your Emacs, you can just install *window-shaper* with

    M-x package-install window-shaper RET

## Usage

Enable *window-shaper-mode* in any buffer to be able to use single keystrokes
to resize windows.

    (window-shaper-mode)

You can also set a key-binding to enable *window-shaper-mode* from any
buffer.

    (global-set-key (kbd "C-x C-#") 'window-shaper-mode)

Once the *window-shaper-mode* is enabled you can use the following shortcuts:

right: increase window width
left: decrease window width
up: increase window height
down: decrease window height
q: disable window-shaper-mode

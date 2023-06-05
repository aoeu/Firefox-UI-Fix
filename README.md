# Installation

## Put files in your profile directory

* In Firefox's address bar, type `about:support`
* Copy the profile directory (something like  `/home/$USER/.mozilla/firefox/*.default-release` )
* `cp user.js /home/$USER/.mozilla/firefox/*.default-release`
* `cp --recursive chrome /home/$USER/.mozilla/firefox/*.default-release/`
* Restart Firefox (if running) 

## Tweak Firefox settings

* In Firefox settings, type `about:config` 
* Search for these named existing settings and alter their values to:
```
browser.fullscreen.autohide false
browser.compactmode.show true
```

If the settings don't exist, it means Firefox has changed. 

# About 

## What this is
This respository is a fork of the `photon-style` [release branch](https://github.com/black7375/Firefox-UI-Fix/tree/photon-style) of [black7375's Firefox-UI-Fix](https://github.com/black7375/Firefox-UI-Fix).

## What this does
These files attempt to make Firefox look more like it did before version 89 when there was some significant and arbitarary UI changes.
Most importantly:
* Adds dividing lines back inbetween Firefox tabs (to make it possible to see where one tab ends and another begins)
* Moves the colored bars of container tabs back to the bottom of the tab (so they aren't harder to see by the screen bezel)

## Goals of this fork
* __Focus__ - Only provide the Photon (old Firefox) styling and nothing else (as a separation of concerns from providing the Proton and Lepton styling).
* __Clarity__ - pRoton (new Firefox UI) and pHoton (old Firefox UI) are similary named and easy to confuse, and adding another style named Lepton into the mix didn't help.
* __Simplicity__ - Many branches, pages of documentation (that arbitrarily swap pRoton and pHoton order when listed, or sometimes don't clarify what they are), and extra files make it difficult to see the handful of files and folders that merely need to be copied into the Firefox profile directory.

## License
As per requirements of the Mozilla Public License Version 2.0 of the code this reposistory is forked from, you can read and obtain a copy of the [license on Mozilla's website](https://www.mozilla.org/en-US/MPL/2.0/).

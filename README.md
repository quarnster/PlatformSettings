# Description

This is a [Sublime Text 2](http://www.sublimetext.com) plugin enabling platform specific settings.

# Installation

* The easiest way to install PlatformSettings is via the excellent Package Control Plugin
    * **NOTE** at the time of writing this, it's not in the default Package Control channel. Please add it via
        1. Open up the command palette
        2. Select "Package Control: Add Repository"
        3. Type https://github.com/quarnster/PlatformSettings
    1. See the [Package Control Installation Instructions](http://wbond.net/sublime_packages/package_control/installation)
    2. Once package control has been installed, bring up the command palette (cmd+shift+P or ctrl+shift+P)
    3. Type Install and select "Package Control: Install Package"
    4. Select PlatformSettings from the list. Package Control will keep it automatically updated for you
* If you don't want to use package control, you can manually install it
    1. Go to your packages directory and type:
    2.    git clone https://github.com/quarnster/PlatformSettings

# Usage

Add a key to your settings dictionary like the following:

    "osx":
    {
        "font_size": "12.0"
    },
    "linux":
    {
        "font_size": "10.0"
    },
    "windows":
    {
        "font_size": "8.0"
    }


Each setting in the platform specific dictionary will be applied to your views if they are different from what is currently set.

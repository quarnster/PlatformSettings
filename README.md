# Description

This is a [Sublime Text 2](http://www.sublimetext.com) plugin enabling platform specific settings.

# Installation

* The easiest way to install PlatformSettings is via the excellent Package Control Plugin
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
        "font_size": 12.0
    },
    "linux":
    {
        "font_size": 10.0
    },
    "windows":
    {
        "font_size": 8.0
    }


Each setting in the platform specific dictionary will be applied to your views if they are different from what is currently set.

You can also specify which keys you want to apply (and in what order) to your settings:

    "platform_settings_keys": ["${platform}", "user_${platform}"]

This is the default setting, so if you are using OS X the dictionary with the name "osx" will be loaded and then updated with the settings from the dictionary with the name "user_osx" before being applied to your views.


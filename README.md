CyanogenMod Dev Center
==========

CMDC GUI

Make sure debhelper is installed:

    sudo apt-get install debhelper

Now download the code , build and install.

    git clone git@github.com:lithid/CMDC.git
    dpkg-buildpackage -rfakeroot
    sudo dpkg -i ../cmdc_0.{VERSION}_amd64.deb

Note: dpkg alone doesn't handle dependancies. If you need to install them use this command.

    sudo apt-get install -f

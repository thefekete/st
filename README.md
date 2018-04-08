# st - simple terminal
**st** is a simple terminal emulator for X which sucks less. 

# Deviations
This is a fork of **st** and therefore sucks a little more than the original in the following ways:

* Changes default font pixelsize to 18
* Applies [patches for scrollback](https://st.suckless.org/patches/scrollback/) with mouse wheel and Page Up / Down keys
* Shamelessly rips off the [patches for Solarized color switching](https://st.suckless.org/patches/solarized/) with modifications and slight tweaks

Another addition is the documentation of the new mouse/keyboard shortcuts and command line options from patches or my own changes to the st.1 man page.


# Requirements
In order to build st you need the Xlib header files.


# Installation
Edit config.mk to match your local setup (st is installed into the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if necessary as root):

    make clean install

# Documentation
Check out the source to see how things work. Read the **st(1)** man page for a quick overview of available options.


# Running st
If you did not install st with make clean install, you must compile the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

# Credits
This is a fork of the [suckless simple terminal project](https://st.suckless.org/) which is based on Aurélien APTEL <aurelien dot aptel at gmail dot com>'s bt source code.


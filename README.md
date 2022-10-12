# rustdesk-bin package for Void Linux

This package provides Rustdesk, open source virtual / remote desktop infrastructure, TeamViewer alternative.. This package merely takes the .deb release version from the authors, extracts and installs the files as is. **Note:** This is not building binaries from source as a proper package should. Hence the `-bin` shuffix.

The template file is prepared for use with [xbps-src](https://wiki.voidlinux.org/Xbps-src) in Void Linux.

## Runtime dependencies

1. `python3` (`pynput` package)
2. `xdotool`

## Installation
```
git clone https://github.com/void-linux/void-packages
cd void-packages
./xbps-src binary-bootstrap
# Do the above once if not done already.
# Copy this `rustdesk-bin` folder under `srcpkgs` folder, then...

# Install dependencies
pip install pynput
sudo xbps-install xdotool

# Install rustdesk-bin
./xbps-src pkg rustdesk-bin
sudo xbps-install --repository hostdir/binpkgs brave-bin
```

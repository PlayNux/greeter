# Starter


## Building and Installation

You'll need the following dependencies:

* gnome-settings-daemon >= 3.27
* libaccountsservice-dev
* libgdk-pixbuf2.0-dev
* libgranite-dev >= 5.5.0
* libgtk-3-dev
* libhandy-1-dev >= 0.90.0
* liblightdm-gobject-1-dev
* libmutter-6-dev
* libx11-dev
* meson
* valac

Run `meson` to configure the build environment and then `ninja` to build

    meson build --prefix=/usr
    cd build
    ninja

To install, use `ninja install`

    sudo ninja install

## Testing & Debugging

Run LightDM in test mode with Xephyr:

    lightdm --test-mode --debug

You can then find the debug log in `~/.cache/lightdm/log`

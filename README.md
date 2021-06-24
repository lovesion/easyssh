[![Translation status](https://hosted.weblate.org/widgets/easyssh/-/translations/svg-badge.svg)](https://hosted.weblate.org/engage/easyssh/?utm_source=widget)

<h1 align="center">EasySSH</h1>

## The SSH connection manager to make your life easier.
## Using zsh and zssh to make your life easier and easier.
## Thanks to the project 'easyssh'!

A complete, efficient and easy-to-use manager. Create and edit connections, groups, customize the terminal, with multiple instances of the same connection.

### Features

* Manage connections and groups
* Customize terminal
* Dark Theme
* Multiple instances of same connection
* Restore opened hosts
* Sync `~/.ssh/config`
* Protect data with password

### Donate
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=YQ7R5KQJPUNNU&currency_code=BRL&source=url">PayPal</a> | <a href="https://www.patreon.com/muriloventuroso">Patreon</a>

![Screenshot](data/screenshot.png)

![Screenshot](data/screenshot2.png)


## Developing and Building

If you want to hack on and build EasySSH yourself, you'll need the following dependencies:

* libgee-0.8-dev
* libgtk-3-dev
* libgranite-dev
* libvte-2.91-dev
* libjson-glib-dev
* meson
* valac
* gpg
* zsh
* lrzsz
* zssh

Run `meson build` to configure the build environment and run `ninja test` to build and run automated tests

    meson build --prefix=/usr
    cd build
    ninja test

To install, use `ninja install`, then execute with `com.github.muriloventuroso.easyssh`

    sudo ninja install
    com.github.muriloventuroso.easyssh

Pacman-based(Arch/Manjaro/Others) :
```
 meson build --prefix=/usr -D libunity=false -D ubuntu-bionic-patched-vte=false -D patched-vte=true
 ninja -C build install
```

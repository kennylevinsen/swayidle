# swayidle

This is sway's idle management daemon, swayidle. It is compatible with any
Wayland compositor which implements the KDE
[idle](https://github.com/swaywm/sway/blob/master/protocols/idle.xml) protocol.
See the man page, [swayidle(1)](./swayidle.1.scd), for instructions on configuring swayidle.

## Release Signatures

Releases are signed with [34FF9526](https://keys.openpgp.org/search?q=34FF9526CFEF0E97A340E2E40FDE7BE0E88F5E48)
and published [on GitHub](https://github.com/swaywm/swayidle/releases). swayidle
releases are managed independently of sway releases.

## Installation

### From Packages

Swayidle is available in many distributions. Try installing the "swayidle"
package for yours.

If you're interested in packaging swayidle for your distribution, stop by the
IRC channel or shoot an email to sir@cmpwn.com for advice.

### Compiling from Source

Install dependencies:

* meson \*
* wayland
* wayland-protocols \*
* [scdoc](https://git.sr.ht/~sircmpwn/scdoc) (optional: man pages) \*
* git \*

_\*Compile-time dep_

Run these commands:

    meson build
    ninja -C build
    sudo ninja -C build install

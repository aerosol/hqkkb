# hqkkb

![hqkkb](https://user-images.githubusercontent.com/173738/71843051-51f52e00-30c3-11ea-9bc8-2feae2ac355f.jpeg)

This is a newb attempt at tuning NPKC's HHKB firmware to better reflect the original PFU HHKB2 layout.

I only updated selected mappings I frequently use on the original PFU board.
This repo does not aim to be a proper QMK ecosystem citizen, yet.

Make example for this keyboard (after setting up your build environment):

    make hqkkb:default

ArchLinux flashing hints:
  - use [QMK's Vagrant](https://beta.docs.qmk.fm/detailed-guides/getting_started_vagrant)
  - add yourself to `vboxusers` group
  - install `aur/virtualbox-ext-oracle`
  - verify the board is seen on guest with:
      - `vagrant ssh -c 'sudo -i'`
      - `apt install usbutils`
      - `lsusb`
  - flash with `make hhkb:default:dfu` after entering QMK programming mode (<kbd>fn+z</kbd>)

Successfully flashed device should be seen as:

```
Bus 001 Device 018: ID dead:beef NPKC HQKKB aerosol
```


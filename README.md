# RTL8812BU / RTL8822BU driver for Linux

This is a Linux driver for Realtek RTL8812BU / RTL8822BU based devices. This is a driver for the wireless part *only* (no Bluetooth).

This driver is known to support Linksys WUSB6400M (based on RTL8812BU?).

## Building

Build and install (requires `dkms`):

```sh
sudo make -f Makefile.dkms install
```

Uninstall:

```sh
sudo make -f Makefile.dkms uninstall
```

## Loading the driver

Reboot your system, or if you're impatient:

```sh
sudo modprobe -a rtl8822bu
```

## Credits

This is a fork of [ulli-kroll/rtl8822bu](https://github.com/ulli-kroll/rtl8822bu), by Hans Ulli Kroll.

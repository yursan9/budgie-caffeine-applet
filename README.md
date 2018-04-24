# Budgie Caffeine Applet

Simple applet to prevent screen dimming on long idle time.

![The applet](https://raw.githubusercontent.com/yursan9/budgie-caffeine-applet/master/img/initial-applet.png)

## Feature

- Prevent screen dimming
- Prevent triggering lock screen
- Notification support (For you who want visual noise)
- Single click activation with middle mouse button
- Timer
- i18n Support

![notification support](https://raw.githubusercontent.com/yursan9/budgie-caffeine-applet/master/img/notification-support.png)

## Requirement

- budgie-1.0 >= 2
- gobject-introspection
- gtk3 >= 3.20
- libnotify (notify-send)
- meson
- ninja
- python-gobject
- python3

## Installation

### Solus

```
eopkg it budgie-caffeine-applet
```

### Manual

To install this applet, follow instruction below:
```
git clone https://github.com/yursan9/budgie-caffeine-applet
cd budgie-caffeine-applet
meson builddir --prefix=/usr
cd builddir
```

After that, we'll install the applet with command below
```
sudo ninja install
```

If you want to remove the applet, use `sudo ninja uninstall`.

## Translation

Help me deliver this applet to wider audiences by helping me translate this
applet! Go to
https://www.transifex.com/yursans-budgie-applets/budgie-caffeine-applet/
andstart translating.

## Issue

Only `papirus` icon theme support the icons used by this applet. Because of
that, I provided some ugly fallback icon for you. If you think you can make
better icons, I'll merge your PR.

If any other issues arise, let me know!

## Donation

If you like this applet and do not mind buying my daily dosage of milk.
You can donate to me [here via Paypal](https://paypal.me/YurizalS).

*Salam kopi!*

# 💻 Grub2 Theme

## Installation:

Usage:  `sudo ./install.sh [OPTIONS...]`

```
  -t, --theme     theme variant(s)          [clean]       (default is clean)
  -i, --icon      icon variant(s)           [color]       (default is color)
  -s, --screen    screen display variant(s) [1080p|2k|4k|ultrawide|ultrawide2k] (default is 1080p)
  -r, --remove    Remove theme              [clean]       (must add theme name option, default is clean)

  -b, --boot      install theme into '/boot/grub' or '/boot/grub2'
  -g, --generate  do not install but generate theme into chosen directory       (must add your directory)

  -h, --help      Show this help
```

_If no options are used, a user interface `dialog` will show up instead_

### Examples:
 - Install Clean theme on 2k display device:

```sh
sudo ./install.sh -t clean -s 2k
```

 - Install Clean theme into /boot/grub/themes:

```sh
sudo ./install.sh -b -t clean
```

 - Uninstall Clean theme:

```sh
sudo ./install.sh -r -t clean
```

# OpenWrt packages feed

## Usage

This feed can be installed by including this line in the `feeds.conf` file:

```
src-git oxr463 https://github.com/oxr463/openwrt-packages
```

To install all its package definitions, run:

```
./scripts/feeds update oxr463
./scripts/feeds install -a -p oxr463
```

## License

SPDX-License-Identifier: [GPL-2.0-or-later](https://spdx.org/licenses/GPL-2.0-or-later.html)


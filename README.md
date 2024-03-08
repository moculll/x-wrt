![OpenWrt logo](https://raw.githubusercontent.com/x-wrt/com.x-wrt/master/x-wrt-logo/x-wrt-logo-Aldrich-raw.svg)

This project is for 华正易尚 ES-M6+

Developed from wg3526-32m


### Requirements

```
binutils bzip2 diff find flex gawk gcc-6+ getopt grep install libc-dev libz-dev
make4.1+ perl python3.7+ rsync subversion unzip which
```

### Quickstart
1. Run `git clone https://github.com/moculll/x-wrt.git`

1. Run `./scripts/feeds update -a` to obtain all the latest package definitions
   defined in feeds.conf / feeds.conf.default

2. Run `./scripts/feeds install -a` to install symlinks for all obtained
   packages into package/feeds/

3. Run `git submodule update` to clone argon theme which is default for this X-wrt repo

3. Run `make menuconfig` to select your preferred configuration for the
   toolchain, target system & firmware packages.

4. Run `make` to build your firmware. This will download all sources, build the
   cross-compile toolchain and then cross-compile the GNU/Linux kernel & all chosen
   applications for your target system.

## License

OpenWrt is licensed under GPL-2.0

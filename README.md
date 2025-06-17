# OpenWrt packages feed

## Changes compared to upstream

This custom branch contains several unaccepted PRs of the upstream, as the PR review process is quite slow and some of the PRs are not accepted for a long time :(.

- [PR](https://github.com/openwrt/packages/pull/26531): update `miniupnpd` to 2.3.9 to support `ignore_private_ip_check`
- [PR](https://github.com/openwrt/packages/pull/26659): update `vim` to 9.1.1456 to support github copilot
    - Change `vim-fuller` to as `huge` build to support `+terminal` feature

## Usage

Download the corresponding platform OpenWrt SDK and following the official SDK usage document to setup, then add this feed to the `feeds.conf.default` file

---

## Description

This is the OpenWrt "packages"-feed containing community-maintained build scripts, options and patches for applications, modules and libraries used within OpenWrt.

Installation of pre-built packages is handled directly by the **opkg** utility within your running OpenWrt system or by using the [OpenWrt SDK](https://openwrt.org/docs/guide-developer/using_the_sdk) on a build system.

## Usage

This repository is intended to be layered on-top of an OpenWrt buildroot. If you do not have an OpenWrt buildroot installed, see the documentation at: [OpenWrt Buildroot – Installation](https://openwrt.org/docs/guide-developer/build-system/install-buildsystem) on the OpenWrt support site.

This feed is enabled by default. To install all its package definitions, run:
```
./scripts/feeds update packages
./scripts/feeds install -a -p packages
```

## License

See [LICENSE](LICENSE) file.
 
## Package Guidelines

See [CONTRIBUTING.md](CONTRIBUTING.md) file.

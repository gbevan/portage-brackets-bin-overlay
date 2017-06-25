Gentoo Portage Overlay for the Brackets Code Editor
===================================================

**This project is deprecated in favour of the [Brackets-Electron Gentoo Portage Overlay](https://github.com/gbevan/brackets-electron-bin-overlay).**


Configuration
-------------

/etc/layman/layman.cfg add:

    overlays: ...
              https://github.com/gbevan/portage-brackets-bin-overlay/raw/master/repository.xml

```bash
layman -f -a gbevan-brackets

emerge -v --ask brackets-bin
```

Upgrade
-------

```bash
layman -S

eix-update

emerge -v --ask -u brackets-bin
```

Developer Notes:
----------------

* When releasing new ebuild, run:

        ebuild brackets-bin-?.?.ebuild manifest

  for your new ebuild version, then commit/push.

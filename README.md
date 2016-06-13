Gentoo Portage Overlay for the Brackets Code Editor
===================================================

Configuration
-------------

/etc/layman/layman.cfg add:

    overlays: ...
              https://github.com/gbevan/portage-brackets-bin-overlay/raw/master/repository.xml

layman -f -a gbevan-brackets

emerge -v --ask brackets-bin

Upgrade
-------

layman -S

emerge -v --ask -u brackets-bin

Developer Notes:
----------------

* When releasing new ebuild, run:

        ebuild brackets-bin-?.?.ebuild manifest

  for your new ebuild version, then commit/push.

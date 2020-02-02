List of applications working with Wayland natively
===================================================

This list is not intended to be always current or complete.
Support is being added in new applications all the time.

* Applications using GTK3+, SDL2+, and Qt5+ generally always have support when those libraries are compiled with the `wayland` package option.
* FreeGLUT has support but it only supports one backend at a time (for now), so you have to disable x11 support.
* GLEW does not yet have usable support. Some applications using GLEW can fall back and still work. blastem is one of these.
* For Qt, `export QT_QPA_PLATFORM=wayland-egl` must be set in the environment.
  Make sure `x11/qt5-qtwayland` is installed.

Obviously this list doesn't include curses-based CLI applications, which will always work in the terminal emulator of your choice.

If you want to try 3D support out, install `graphics/MesaDemos` and run `eglgears_wayland` or `eglinfo`. Make sure MesaLib is compiled with the wayland option and you have `PREFER_PKGSRC=MesaLib` in `mk.conf` (probably glu and libepoxy too).

**TODO:** LibreOffice, Mozilla stuff, Input methods...

Audio players
-------------

* audio/exaile (GTK, use dbus-launch)
* audio/quodlibet (GTK)
* audio/rhythmbox (GTK, use dbus-launch)

Audio players (musicpd clients)
-------------------------------

* audio/ario (GTK)
* audio/cantana (Qt)
* audio/sonata (GTK)

Audio editors
-------------

* audio/audacity (GTK)
* audio/fasttracker2 (SDL)
* audio/lmms (Qt)
* audio/milkytracker (SDL)
* audio/musescore (Qt)

Video players
-------------

* multimedia/mpv (Independent) **[Recommended]**
	- Use `--vo=gpu --gpu-context=wayland`, or add it to `$HOME/.config/mpv/mpv.conf` without the leading dashes
* multimedia/ffplay (SDL)
* multimedia/vlc (Qt)

Video editors
-------------

* multimedia/olive-editor (Qt)
* multimedia/pitivi (GTK)

Image editors
-------------

* graphics/krita (Qt)

Web browsers
------------

* www/midori (GTK, WebKit)
* www/netsurf (GTK)
* www/otter-browser (Qt, WebKit)
* www/vimb (GTK, WebKit, vi-ish)

Office
------

* editors/abiword (GTK)
* editors/lyx (Qt)
* math/gnumeric (GTK)

Feed readers
-------------

* www/liferea (GTK)

E-book readers
--------------

* print/foliate **[Recommended]**
* print/mupdf (GLUT, build with opengl + build freeglut with wayland)
* misc/calibre (Qt)

PDF readers
-----------

* print/evince (GTK)
* print/dspdfviewer (Qt)
* print/mupdf (GLUT, build with opengl + build freeglut with wayland)
* print/qpdfview (Qt) **[Recommended]**
* print/xpdf4 (Qt)
* print/xournalpp (Qt, PDF annotator)
* print/zathura (GTK, vi-ish)

Image viewers
-------------

* graphics/imv (Independent) **[Recommended]**
* graphics/ristretto (GTK)
* graphics/geeqie (GTK)

Terminal emulators
------------------

* x11/sakura (GTK) **[Recommended]**
* x11/xfce4-terminal (GTK)

Text editors
------------

* editors/gedit (GTK)
* editors/l3afpad (GTK)
* editors/tea (Qt)
* editors/xfce4-mousepad (GTK, use dbus-launch)

File managers
-------------

* sysutils/xfce4-thunar (GTK)
* sysutils/gentoo (GTK)

Archive managers
----------------

* sysutils/xfce4-xarchiver (GTK)

Calculators
-----------

* math/galculator (GTK)

Email clients
-------------

* mail/balsa (GTK)
* mail/evolution (GTK)

IRC clients
-----------

* chat/quassel (Qt)

File transfer
-------------

* net/filezilla (GTK)
* net/transmission-gtk (GTK)
* net/transmission-qt (Qt)

CAD
---

* cad/librecad (Qt)
* cad/openscad (Qt)
* cad/qcad (Qt)

Password managers
-----------------

* security/keepassxc (Qt)

Databases
---------

* databases/sqlitebrowser (Qt)

Games
------

* games/REminiscence (SDL)
* games/7kaa (SDL)
* games/astromenace (SDL)
* games/cataclysm-dda-sdl (SDL)
* games/chocolate-doom (SDL)
* games/devilutionx (SDL)
* games/dunelegacy (SDL)
* games/easyrpg-player (SDL)
* games/etlegacy (SDL)
* games/flare-game (SDL)
* games/freeciv-client (GTK)
* games/gemrb (SDL)
* games/iortcw (SDL)
* games/lugaru (SDL)
* games/manaplus (SDL)
* games/naev (SDL)
* games/neverball (SDL)
* games/openjk (SDL)
* games/openmw (SDL)
* games/openrtc2 (SDL)
* games/oshu (SDL)
* games/redeclipse (SDL)
* games/solarus (SDL)
* games/srb2 (SDL)
* games/powder-toy (SDL)
* games/simutrans (SDL)
* games/quakespasm (SDL)
* games/stone-soup-sdl (SDL)
* games/vvvvvv (SDL)
* games/wesnoth (SDL)
* games/xonotic (SDL)
* games/yquake2 (SDL)

Emulators
---------

* emulators/aranym (SDL)
* emulators/blastem (SDL)
* emulators/dolphin-emu (GTK/SDL)
* emulators/dosbox-x (SDL)
* emulators/fuse-emulator (GTK)
* emulators/fs-uae (SDL)
* emulators/hatari (SDL)
* emulators/mame (SDL)
* emulators/mednafen (SDL)
* emulators/mednaffe (GTK)
* emulators/melonds (GTK/SDL)
* emulators/mgba (Qt)
* emulators/nestopia (GTK/SDL)
* emulators/qemu (GTK/SDL)
* emulators/sameboy (SDL)
* emulators/shoebill (SDL)
* emulators/simh (SDL)
* emulators/snes9x-gtk (GTK/SDL)
* emulators/stella (SDL)
* emulators/vice (GTK)
* emulators/yabause (Qt)

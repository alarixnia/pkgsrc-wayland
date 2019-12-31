Application configuration
=========================

## Forcing use of the Wayland backend

### GTK+

~~~
$ export GDK_BACKEND=wayland
~~~

### Qt

~~~
$ export QT_QPA_PLATFORM=wayland-egl
~~~

### SDL

~~~
$ export SDL_VIDEODRIVER=wayland
~~~

### Mozilla software (e.g. Firefox)

~~~
$ export MOZ_ENABLE_WAYLAND=1
~~~

## GTK appearance

Configure the appearance of GTK applications by running `gsettings` on startup.

~~~
$ gsettings set org.gnome.desktop.interface gtk-theme 'Materia-compact'
$ gsettings set org.gnome.desktop.interface icon-theme 'Papirus'
$ gsettings set org.gnome.desktop.interface cursor-theme 'Vanilla-DMZ-AA'
$ gsettings set org.gnome.desktop.interface font-name 'Koruri 11'
$ gsettings set org.gnome.desktop.interface monospace-font-name 'Inconsolata 11'
$ gsettings set org.gnome.desktop.interface gtk-key-theme 'Emacs'
~~~

You can do `export DESKTOP_SESSION=gnome` if you want some of these settings to apply to Qt
applications.

## HiDPI

If you have a HiDPI screen, you can use the following environment variables to scale screen elements:

~~~
$ export QT_SCALE_FACTOR=2
$ export GDK_DPI_SCALE=2
~~~

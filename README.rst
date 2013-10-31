Android Utils
=============

Some command-line tools to make developing Android apps a bit easier. All tools
are badly documented, but some help may be obtained by running the tool with
--help.


dippy
-----

A utility for converting dps to px in various pixel-densities, and vice-versa.

::

    $ dippy 128 dp
    128.0 dp
    ========
    xxhdpi : 384.0 px
    xhdpi  : 256.0 px
    hdpi   : 192.0 px
    mdpi   : 128.0 px
    ldpi   : 96.0 px

::

    128.0 px (xhdpi) = 64.0 dp
    ==========================
    xxhdpi : 192.0 px
    xhdpi  : 128.0 px
    hdpi   : 96.0 px
    mdpi   : 64.0 px
    ldpi   : 48.0 px


res-copy
--------

A tool for correctly copying resources into an Android project's res directory.

At present, this is probably the most useful tool in the toolbox, but the
command-line interface is still in flux, so I don't want to document it yet.


res-cmp
-------

A tool for comparing a set of drawable directories to ensure that resource files
have been added to all of them.

::

    $ res-cmp res/drawable-*
    btn_check_on_holo_light.png is missing in drawable-xxhdpi
    btn_check_on_pressed_holo_light.png is missing in drawable-xxhdpi
    btn_current_location_disabled.png is missing in drawable-hdpi, drawable-mdpi and drawable-xxhdpi
    btn_current_location_normal.png is missing in drawable-xxhdpi
    btn_current_location_pressed.png is missing in drawable-xxhdpi


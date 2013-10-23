=====
dippy
=====

A command-line tool for converting values between dp and px at different
pixel-densities.

.. code-block:: none

    $ dippy 72dp

    72.0 dp
    =======
    xxhdpi : 216.0 px
    xhdpi  : 144.0 px
    hdpi   : 108.0 px
    mdpi   : 72.0 px
    ldpi   : 54.0 px

The one argument is a size and can be provided in dp, or in pixels, specified
by pixel-density - one of xxhdpi, xhdpi, hdpi, mdpi or ldpi.
========
res-copy
========

res-copy copies finds and copies resources to the correct locations in an
Android project's res structure.

.. code-block:: none

    usage: res-copy [-h] [-v] [-d] [-f] srcroot destroot [pattern [pattern ...]]

    positional arguments:
      srcroot
      destroot
      pattern

    optional arguments:
      -h, --help     show this help message and exit
      -v, --verbose
      -d, --dry-run
      -f, --force

res-copy searches for png and jpg files beneath srcroot, identifies the
pixel-density of the resource from the file's path or filename, and then copies
the resource to the correct folder beneath destroot.

To determine a resource's pixel density, the path is checked for one of xxhdpi,
xhdpi, hdpi, mdpi and ldpi. If the filename contains one of the specifiers,
preceded by a hyphen, an underscore, or a space, the filename will have this
stripped before copying.
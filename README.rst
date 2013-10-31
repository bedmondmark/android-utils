Android Utils
=============

Some command-line tools to make developing Android apps a bit easier. All tools
are badly documented, but some help may be obtained by running the tool with
--help.


dippy
-----

A utility for converting dps to px in various pixel-densities, and vice-versa.


res-copy
--------

A tool for correctly copying resources into an Android project's res directory.


res-cmp
-------

A tool for comparing a set of drawable directories to ensure that resource files
have been added to all of them. ::

    $ res-cmp res/drawable-*

... will tell you which resource files are missing from a subset of your
drawable directories.

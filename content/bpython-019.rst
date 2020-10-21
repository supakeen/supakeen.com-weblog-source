Release of bpython 0.19
#######################

:date: 2020-03-27 12:00
:tags: python, bpython
:category: python
:slug: bpython-019
:authors: supakeen
:summary: About the release of bpython 0.19

bpython_ 0.19 was just released. You can get it from PyPI_ or check out our
GitHub_. The changelog was as follows:

0.19
****

General information
===================

* The bpython-cli and bpython-urwid rendering backends have been deprecated and will show a warning that they'll be removed in a future release when started.
* Usage in combination with Python 2 has been deprecated. This does not mean that support is dropped instantly but rather that at some point in the future we will stop running our testcases against Python 2.
* The new pinnwand API is used for the pastebin functionality. We have dropped two configuration options: `pastebin_show_url` and `pastebin_removal_url`. If you have your bpython configured to run against an old version of `pinnwand` please update it.

Fixes
=====

* #765: Display correct signature for decorated functions. Thanks to Benedikt Rascher-Friesenhausen.
* #776: Protect get_args from user code exceptions
* Improve lock file handling on Windows
* #791: Use importlib instead of deprecated imp when running under Python 3

Support for Python 3.8 has been added. Support for Python 3.4 has been dropped.


.. _bpython: https://bpython-interpreter.org/
.. _PyPI: https://pypi.org/project/bpython/
.. _GitHub: https://github.com/bpython/bpython

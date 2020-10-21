Release of bpython 0.20
#######################

:date: 2020-10-20 12:00
:tags: python, bpython
:category: python
:slug: bpython-020
:authors: supakeen
:summary: About the release of bpython 0.20

bpython_ 0.20 was just released. You can get it from PyPI_ or check out our
GitHub_. The changelog was as follows:

0.20
****

General information
===================

* The next release of bpython (0.20) will drop support for Python 2.
* Support for Python 3.9 has been added. Support for Python 3.5 has been
  dropped.

New features
============

* #802: Provide redo.
  Thanks to Evan.
* #835: Add support for importing namespace packages.
  Thanks to Thomas Babej.

Fixes
=====

* #622: Provide encoding attribute for FakeOutput.
* #806: Prevent symbolic link loops in import completion.
  Thanks to Etienne Richart.
* #807: Support packages using importlib.metadata API.
  Thanks to uriariel.
* #809: Fix support for Python 3.9's ast module.
* #817: Fix cursor position with full-width characters.
  Thanks to Jack Rybarczyk.
* #853: Fix invalid escape sequences.

.. _bpython: https://bpython-interpreter.org/
.. _PyPI: https://pypi.org/project/bpython/
.. _GitHub: https://github.com/bpython/bpython

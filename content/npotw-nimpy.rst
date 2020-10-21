Nim Package of the Week: npeg
##############################

:date: 2020-10-26 12:00
:tags: nim, npotw, nimpy
:category: nim
:slug: npotw-nimpy
:authors: supakeen
:summary: Nim package of the week nimpy

nimpy_ is a package for Nim_ to allow bidirectional integration between Python
and Nim. This lets you write functions in Nim and call them from Python and
vice versa.

I've used ``nimpy`` several times to speed up tight loops or together with last
weeks NPOTW npeg_ to write fast parsers to use from Python without having to
get down and dirty in C.

Examples speak more than words, here is a ``nimpy`` example from its README:

.. code-block:: nimrod

        # mymodule.nim - file name should match the module name you're going to import from python
        import nimpy

        proc greet(name: string): string {.exportpy.} =
          return "Hello, " & name & "!"

When you build the above module with ``nim c --threads:on --app:lib --out:mymodule.so mymodule``
and then place it on your import path for Python you can use it:

.. code-block:: python

        import mymodule
        assert mymodule.greet("world") == "Hello, world!"
        assert mymodule.greet(name="world") == "Hello, world!"

The offered speedups to get C speed of execution while still having a higher
level language to write your code in should lessen the step when deciding to
fork out some performance critical bits of your Python to another language!

The Nim Package of the Week is a series on Nim packages that make up the
ecosystem where a new article appears weekly on a library that you should
know about.

.. _nimpy: https://github.com/yglukhov/nimpy
.. _npeg: https://supakeen.com/weblog/npotw-npeg.html
.. _Nim: https://nim-lang.org/

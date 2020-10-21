Nim Package of the Week: npeg
##############################

:date: 2020-10-20 20:00
:tags: nim, npotw, npeg
:category: nim
:slug: npotw-npeg
:authors: supakeen
:summary: Nim package of the week npeg.

npeg_ is a package for Nim_ implementing PEGs_ or Parser Expression Grammars.
This allows you to express complex parsing operations in a semi-standardized
and concise manner while offering more flexibility than Regular Expressions
have.

Examples speak more than words, here is an ``npeg`` example from its README:

.. code-block:: nimrod

		import npeg, strutils, tables

		type Dict = Table[string, int]

		let parser = peg("pairs", d: Dict):
		  pairs <- pair * *(',' * pair) * !1
		  word <- +Alpha
		  number <- +Digit
		  pair <- >word * '=' * >number:
			d[$1] = parseInt($2)

		var words: Table[string, int]
		doAssert parser.match("one=1,two=2,three=3,four=4", words).ok
		echo words

The above parses the string ``one=1,two=2,three=3,four=4`` into a ``Dict`` by
key and value.

Aside from providing nice macros and syntax to define PEGs the ``npeg`` package
also contains one of the most complete READMEs dense with information on how
to write and handle PEGs for parsing.

The Nim Package of the Week is a series on Nim packages that make up the
ecosystem where a new article appears weekly on a library that you should
know about.

.. _npeg: https://github.com/zevv/npeg
.. _Nim: https://nim-lang.org/
.. _PEGs: https://en.wikipedia.org/wiki/Parsing_expression_grammar

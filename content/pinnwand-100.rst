Pinnwand 1.0.0 and its history
##############################

:date: 2020-03-27 12:00
:tags: python, pinnwand
:category: python
:slug: pinnwand-100-and-history
:authors: supakeen
:summary: About the release of pinnwand 1.0.0 and its history.

pinnwand_ 1.0.0 was released and shortly thereafter followed by the customary
1.0.1 release to fix that one bug that always gets discovered just after
release. You can download these from PyPI_.

The major features that have been added to the pinnwand 1.0 release are:

* multi-file pastes, pastes can now contain multiple files
* shorter URLs, paste IDs are now more readable and less typo prone
* pinnwand was fully rewritten for Python 3 in the Tornado_ framework.

Together with a slew of smaller changes and bugfixes.

history
*******
I've been asked before to clarify on the history of the pastebin and how it
came to be. This section of the blog post will go into that.

Back when bpython_ was started I was one of its contributors (still am) on a
different nickname. I thought it would be neat if we would add pastebin support
to bpython but to do so I didn't want to be reliant on a 3rd party pastebin.

Back in those days there was another pastebin called LodgeIt, it was ran by the
people behind Pocoo_ and built on the Flask_ framework. I setup my own instance
of this on the bpaste.net_ domain. That name came from the bpython name.

After a while some features (I don't exactly recall which) needed to be added
to bpaste.net and I decided to fork LodgeIt and named it pinnwand. That means
"bulletin board" in English and was fitting for a thing that people put stuff
on for others to see.

In keeping with the theme my other projects that involve pinnwand are named
in similar vein: steck_ (to stick) a client for sticking stuff on the pinnwand
and nagel_ (a thumbtack) as the library to interface with the pinnwand.

This fork then went on to be hosted at both bpaste.net and on a separate domain
for the #python channel on Freenode. Someone else maintained that instance of
pinnwand. The pastebin recommended in the channel flip flopped between the
channel instance and bpaste.net.

A few years later I rekindled my love for the project and decided to start from
scratch. With this a lot of history was lost but here we are at version 1.0.0
and here to stay!

.. _pinnwand: https://supakeen.com/project/pinnwand/
.. _nagel: https://supakeen.com/project/nagel/
.. _steck: https://supakeen.com/project/steck/
.. _PyPI: https://pypi.org/project/pinnwand/
.. _tornado: https://tornadoweb.org/
.. _bpython: https://bpython-interpreter.org/
.. _pocoo: https://pocoo.org/
.. _Flask: https://palletsprojects.com/p/flask/
.. _bpaste.net: https://bpaste.net/

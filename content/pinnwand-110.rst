Release of pinnwand 1.1.0
#########################

:date: 2020-05-24 12:00
:tags: python, pinnwand
:category: python
:slug: pinnwand-110
:authors: supakeen
:summary: About the release of pinnwand 1.1.0

pinnwand_ 1.1.0 has been released. The changelog is as follows:

* Provide a button to toggle line wrapping, contributed by Kwpolska_. (#51)
* Auto-delete pastes on view when they've expired. (#63)
* Include original filename if given for paste downloads (#26)
* Provide a button to toggle opposite colorschemes. (#69)
* For pastes the first file will now have the same slug as the paste itself,
  this allows for users to replace part of the URL to get to raw and download
  links. (#64)
* Allow access to raw and download handlers through /:id/(raw|download) to
  let people more easily change the URL by hand when linked to a paste (#72)
* Consolidate separate pygments and pinnwand stylesheets into one.


.. _pinnwand: https://supakeen.com/project/pinnwand/
.. _Kwpolska: https://github.com/Kwpolska

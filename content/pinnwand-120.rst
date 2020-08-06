Release of pinnwand 1.2.0
#########################

:date: 2020-08-06 12:00
:tags: python, pinnwand
:category: python
:slug: pinnwand-120
:authors: supakeen
:summary: About the release of pinnwand 1.2.0

pinnwand_ 1.2.0 has been released. The changelog is as follows:

New features all around, minor bugfixes, code quality improvements.

* Add language autodetection, contributed by mweinelt_. (#83)
* Provide a hex view for pastes. (#86)
* Add copy to clipboard button. (#87)
* Command line option (-v) to change log level. (#88)
* Make the outline color of the focused form elements be in-line with the
  general highlight color.
* Sum up filesizes and check against paste size. This change now makes the
  paste size limit the total size, not a per-file limit! Adjust your
  configuration accordingly. (#89)
* Add a report link for files that may be problematic, this link will be
  added only if the ``report_email`` field is set to anything than None in the
  configuration file, contributed by Bruce1347_ (#2)
* Expanded testcase coverage for website from 69% to 84% by adding and fixing
  broken testcases.

.. _pinnwand: https://github.com/supakeen/pinnwand
.. _mweinelt: https://github.com/mweinelt
.. _Bruce1347: https://github.com/Bruce1347

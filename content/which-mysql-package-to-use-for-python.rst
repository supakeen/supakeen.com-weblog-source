Which mysql package to use for Python
#####################################

:date: 2020-01-11 12:00
:tags: python
:category: python
:slug: 0x05
:authors: supakeen
:summary: Which mysql package to use for Python.

A commonly asked question in many a Python support channel is which of the
half dozen (or more) mysql packages to use. It's pretty confusing and I had
to spend some time on it recently.

If you want to be told straight ahead, use mysqlclient_ or pymysql_. For the
reasoning hang in there.

Globally there's a few common packages in use throughout tutorials,
documentation, and othe rplaces you might encounter them. These are:

* MySQLdb_
* mysql.connector_
* oursql_
* mysqlclient_
* pymysql_

I'm skipping over other packages such as aiomysql_ as that one is built on top
of pymysql_.

MySQLdb
-------

mysql.connector
---------------

oursql
------

mysqlclient
-----------

pymysql
-------

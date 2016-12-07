python-scrapinghub release notes
================================

Version 1.9.0 (2016-11-02)
--------------------------

- `python-hubstorage`_ merged into python-scrapinghub
- all tests are improved and rewritten with py.test
- hubstorage tests use vcrpy cassettes, work faster and don't require any external services to run

`python-hubstorage`_ is going to be considered deprecated,
its next version will contain a deprecation warning and a proposal
to use python-scrapinghub >=1.9.0 instead.

1.8.0 (2016-07-29)
--------------------------

- python 3 support & unittests
- add retries on httplib.HTTPException
- update scrapinghub api endpoint

v1.7.0 (2014-07-25)
--------------------------

- basic py3.3 compatibility while keeping py2.7 compatibility
- update setup.py classifiers

Version 1.6.2 (2014-07-01)
--------------------------

- fix travis workaround deploying on tags

Version 1.6.1 (2014-07-01)
--------------------------

- packaging improvements
- cleaner implementation of project.job()

Version 1.6.0 (2014-03-14)
--------------------------

- support retreiving a fixed amount of items

Version 1.5.0 (2014-01-29)
--------------------------

- switch to dash secure endpoint

Version 1.4.4 (2013-12-18)
--------------------------

- log download failure as error only if all attempts exhausted

Version 1.4.3 (2013-11-25)
--------------------------

- update travis config to match travis-ci (pypy updated to 2.2)
- update pypi credentials

Version 1.4.2 (2013-11-25)
--------------------------

- add python 3 to travis-ci matrix

Version 1.4.1 (2013-11-25)
--------------------------

- tox, travis-ci and pypi uploads
- pypi uploads only on Python 2.7 success
- run tests under pypy 2.1 in travis-ci

Version 1.4.0 (2013-09-04)
--------------------------

- add bindings for autoscraping api

Version 1.3.0 (2013-08-26)
--------------------------

- add a way to set starting offset
- suport requesting meta fields

Version 1.2.1 (2013-08-22)
--------------------------

- resume item downloads on network errors

Version 1.2.0 (2013-08-08)
--------------------------

- add support for stopping a job
- project.name is deprecated in favour of project.id
- use stricter arguments for Connection constructor
- point to dash.scrapinghub.com api endpoint by default
- enable streaming with requests >= 1.0

Version 1.1.1 (2012-10-24)
--------------------------

- added automatic retry to items download, when the request fails

Version 1.1 (2012-10-19)
------------------------

- report correct version on user-agent string
- ported to uses Requests library (instead of urllib2)
- added support for gzip transfer encoding to increase API throughput on low
  bandwidth connections
- deprecated first url argument of scrapinghub.Connection object
- added support for loading API key from SH_APIKEY environment variable

Version 0.1 (2011-08-15)
------------------------

First release of python-scrapinghub.


.. _python-hubstorage: https://github.com/scrapinghub/python-hubstorage

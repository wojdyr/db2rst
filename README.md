# db2rst
`db2rst.py` script tries to convert DocBook XML to reST (with Sphinx markup enhancements).

I wrote it to convert [fityk](http://fityk.nieto.pl) manual.
It doesn't handle all DocBook elements, only the ones I [needed](https://github.com/wojdyr/fityk/raw/e0056b1b93c63020ddbf3961a0acf016dd74d810/doc/fitykhelp.xml).
The script should be easy to understand and modify.

lxml library is used for parsing DocBook XML.

It's one-off script from 2009, not really maintained now but hopefully still useful.
It was hosted in SVN on Google Code until 2016, so it's not in a github "network" with
it's forks. Most of the forks [stem from Kurt's fork](https://github.com/kurtmckee/db2rst/network/members).
This branch of evolution can be recognized by functions prefixed with `e_` :-)

In 2013 Gerv from Mozilla forked the original script to convert Bugzilla docs.
It may be a good starting point now:
https://github.com/gerv/bzdocs/blob/master/db2rst.py

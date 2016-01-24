`db2rst.py` script tries to convert DocBook XML to reST (with Sphinx markup enhancements).

I wrote it to convert [fityk](http://fityk.nieto.pl) manual,
it doesn't handle all DocBook elements, only the ones I [needed](https://github.com/wojdyr/fityk/raw/e0056b1b93c63020ddbf3961a0acf016dd74d810/doc/fitykhelp.xml).
[The script](http://code.google.com/p/db2rst/source/browse/trunk/db2rst.py)
should be easy to understand and modify.

Let me know if you improve it (gmail: wojdyr).

lxml library is used for parsing DocBook XML.

**Update:** it's one-off script, not really maintained but hopefully useful.
I wrote it in 2009. In 2011 Kurt published [his modified version](https://github.com/kurtmckee/db2rst), which has been [further forked](https://github.com/EronHennessey/db2rst). This branch of evolution includes refactoring I don't like (although there is nothing wrong with it: added classes and prefixes `e_`), and supports more elements than my original script.

In 2013 Gerv from Mozilla forked the original script to convert Bugzilla docs:
https://github.com/gerv/bzdocs/blob/master/db2rst.py <br>
IMHO this is the best starting point now, but having look at other forks may also help.
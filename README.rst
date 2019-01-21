domoticz_skill
==============

|Licence| |Code Health| |Coverage Status|

+------------------+--------------------+
| Status           | Operating system   |
+==================+====================+
| |Build Status|   | Linux x86\_64      |
+------------------+--------------------+

This skill is for controlling Domoticz with the source voice assistant Mycroft.


Requirements
------------

-  `Python3`_.
-  `Domoticz`_.
-  `Mycroft`_.


Configuration
-------------

Configuration file is back... for me it seems useful specially for users speaking other languages and to avoid same notation in this skill and in Domoticz server. Plus, the server can be remote.
Put your configuration in the file “conf.cfg”.

Located in : domoticz_skill/conf.cfg
The principle is to put the 'what' followed by the 'where' separated by a hyphen :

'what-where' = idx
idx is the device number in Domoticz.

examples :

- temperature-living room = 1 
- flood sensor-bathroom = 2
- all lights-house = 3
- Light-Living room = 4

Mycroft Settings Page
-----

The default settings for the domoticz connection and configuration is the local host without
authentication.  [I have yet to grasp how to use it... for now is not functional]

Usage
-----

In English :

examples device names:

-  Living room light
-  Outside temperature
-  Front door lock

example phrases:

-  Hey Mycroft turn on the living room light
-  Hey Mycroft what is the outside temperature?
-  Hey Mycroft lock the front door
-  Hey Mycroft dim the dining room dimmer 50%


Todo
----

Sync server properties to Mycroft settings.

.. _Python3: https://www.python.org/downloads/
.. _Mycroft: https://mycroft.ai/
.. _Domoticz: https://domoticz.com/


.. |Licence| image:: https://img.shields.io/packagist/l/doctrine/orm.svg
.. |Code Health| image:: https://landscape.io/github/matleses/domoticz_skill/master/landscape.svg?style=flat
   :target: https://landscape.io/github/matleses/domoticz_skill/master
.. |Coverage Status| image:: https://coveralls.io/repos/github/matleses/domoticz_skill/badge.svg?branch=master
   :target: https://coveralls.io/github/matleses/domoticz_skill?branch=master
.. |Build Status| image:: https://travis-ci.org/matleses/domoticz_skill.svg?branch=master
   :target: https://travis-ci.org/matleses/domoticz_skill

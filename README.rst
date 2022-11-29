pyspanet
--------

Python Module to interface with a SpaNet controlled spa

Requires Python 3 with asyncio.

To Install::

  pip install pyspanet

To test::

  python3 pyspanet <ip-of-spa-wifi> <port>

To Use
``````

See ``__main__.py`` for usage examples.

Minimal example::

  import asyncio
  import pyspanet

  spa = pyspanet.SpaNetWifi(spa_host, port)
  await spa.connect()
  asyncio.ensure_future(spa.listen())
  await spa.disconnect()
  return

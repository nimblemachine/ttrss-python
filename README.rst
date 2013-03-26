ttrss-python - A Tiny Tiny RSS client library
=============================================

Have you ever wanted to write a python application to interface with your Tiny Tiny RSS server? Read on! 

At a glance
===========

Getting started is easy! Just download and unpack the source distribution and run ``python setup.py install``
in the base directory. ``pip install`` capabilities will be added soon. 

Usage example:

:: 

    from ttrss.client import TTRClient
    client = TTRClient('http://url-to-rss-installation', 'username', 'super-secret-password', auto_login=True)
    cats = client.get_categories()
    cat = cats[0]
    cat.title
    u'News'
    feeds = cat.feeds()
    feed = feeds[0]
    feed.title
    u'MacRumors: Mac News and Rumors - All Stories'
    headlines = feed.headlines()
    # etc...

More detailed API docs coming soon.


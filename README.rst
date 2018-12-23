
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

#### Important Notes! 
 - There is an issue with Buster when using with ghost 2.9.1, so i had to manually fix it. 
 - to remove buster **sudo pip uninstall buster**
 - to install my version of buster 
**sudo pip install git+https://github.com/ramithuh/buster.git**

#### The FIX -> 

>           modified_text = modified_text.replace('pngg','png')
            modified_text = modified_text.replace('pngng','png')
            modified_text = modified_text.replace('pngpng','png')

            modified_text = modified_text.replace('PNGG','PNG')
            modified_text = modified_text.replace('PNGNG','PNG')
            modified_text = modified_text.replace('PNGPNG','PNG')


            modified_text = modified_text.replace('jpgg','jpg')
            modified_text = modified_text.replace('jpgpg','jpg')
            modified_text = modified_text.replace('jpgjpg','jpg')

            modified_text = modified_text.replace('jpegg','jpeg')
            modified_text = modified_text.replace('jpegeg','jpeg')
            modified_text = modified_text.replace('jpegpeg','jpeg')



Buster
======

Super simple, Totally awesome, Brute force **static site generator for**
`Ghost <http://ghost.org>`__.

Start with a clean, no commits Github repository.

*Generate Static Pages. Preview. Deploy to Github Pages.*

Warning! This project is a hack. It's not official. But it works for me.

The interface
-------------

``setup [--gh-repo=<repo-url>]``

      Creates a GIT repository inside ``static/`` directory.

``generate [--domain=<local-address>] [--github-id=<github-id>]``

      Generates static pages from locally running Ghost instance.

``preview``

      Preview what's generated on ``localhost:9000``.

``deploy``

      Commits and deploys changes static files to Github repository.

``add-domain <domain-name>``

      Adds CNAME file with custom domain name as required by Github
Pages.

Buster assumes you have ``static/`` folder in your current directory (or
creates one during ``setup`` command). You can specify custom directory
path using ``[--dir=<path>]`` option to any of the above commands.

Don't forget to change your blog URL in config.js in Ghost.


The Installation
----------------

Installing Buster is easy with pip:

    $ pip install git+git@github.com:raccoonyy/buster.git#egg=buster


You'll then have the wonderful ``buster`` command available.

You could also clone the source and use the ``buster.py`` file directly.

Requirements
------------

-  wget: Use ``brew install wget`` to install wget on your Mac.
   Available by default on most linux distributions.

-  git: Use ``brew install git`` to install git on your Mac.
   ``sudo apt-get install git`` on ubuntu/debian

The following python packages would be installed automatically when
installed via ``pip``:

-  `docopt <https://github.com/docopt/docopt>`__: Creates beautiful
   command line interfaces *easily*.
-  `GitPython <https://github.com/gitpython-developers/GitPython>`__:
   Python interface for GIT.

Ghost. What?
------------

`Ghost <http://ghost.org/features/>`__ is a beautifully designed,
completely customisable and completely `Open
Source <https://github.com/TryGhost/Ghost>`__ **Blogging Platform**. If
you haven't tried it out yet, check it out. You'll love it.

The Ghost Foundation is not-for-profit organization funding open source
software and trying to completely change the world of online publishing.
Consider `donating to Ghost <http://ghost.org/about/donate/>`__.

Buster?
~~~~~~~

Inspired by THE GhostBusters.

.. figure:: https://upload.wikimedia.org/wikipedia/en/3/32/Ghostbusters_2016_film_poster.png
   :alt: Ghost Buster Movie Poster

   Ghost Buster Movie

Contributing
------------

Checkout the existing
`issues <https://github.com/axitkhurana/buster/issues>`__ or create a
new one. Pull requests welcome!

--------------

*Made with* `jugaad <http://en.wikipedia.org/wiki/Jugaad>`__ *in*
`Dilli <http://en.wikipedia.org/wiki/Delhi>`__.

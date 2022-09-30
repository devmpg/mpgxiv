*******************************
Style
*******************************

All guides are written in simple reStructured text format.  Majority of the functionality needed to contribute to this
source can be found in the `Sphinx RST primer <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_,
Or for more in depth documentation, the full `Sphinx Documentation <https://docutils.sourceforge.io/docs/index.html>`_.

==============================
Documentation Style Guidelines
==============================

This section contains the most commonly used RST functionality and style guidelines throughout this site.

*********
Filenames
*********

Use only lowercase alphanumeric characters and ``-`` (minus) symbol.

Suffix filenames with the ``.txt`` extension.

.. note::

  Usage of ``.rst`` extension is not recommended because:

  * RST files are human-readable text files. Most systems natively recognize
    the ``.txt`` extension and open these files with a text editor. This is
    a good choice.

  * Some programs parse ``.rst`` with `rst2html`, which cannot interpret some
    Sphinx's directives such as ``code-block``. So readers using such programs
    actually lose some content.


***********
Whitespaces
***********

Indentation
===========

Indent with 2 spaces.

Except:

* ``toctree`` directive requires a 3 spaces indentation.

Blank lines
===========

Two blank lines before overlined sections, i.e. before H1 and H2.
One blank line before other sections.
See `Headings`_ for an example.

One blank line to separate directives.

.. code-block:: rst

  Some text before.

  .. note::

    Some note.

Exception: directives can be written without blank lines if they are only one
line long.

.. code-block:: rst

  .. note:: A short note.


***********
Line length
***********

Limit all lines to a maximum of 79 characters.


********
Headings
********

Use the following symbols to create headings:

#. ``#`` with overline
#. ``*`` with overline
#. ``=``
#. ``-``
#. ``^``
#. ``"``

As an example:

.. code-block:: rst

  ##################
  H1: document title
  ##################

  Introduction text.


  *********
  Sample H2
  *********

  Sample content.


  **********
  Another H2
  **********

  Sample H3
  =========

  Sample H4
  ---------

  Sample H5
  ^^^^^^^^^

  Sample H6
  """""""""

  And some text.

If you need more than heading level 4 (i.e. H5 or H6), then you should consider
creating a new document.

There should be only one H1 in a document.


***********
Code blocks
***********

Use the ``code-block`` directive **and** specify the language as plain text to create easily copyable text, e.g. macros

.. code-block:: rst

  .. code-block:: text

    I'm in a transitional period so I don't wanna kill you, I wanna help you. But I can't give you this case, it don't belong to me.

***********
Images
***********

Images can be used with the img directive

.. code-block:: rst

    .. image:: path/to/image.ext


.. image:: img/kick.gif

`Image source <https://www.reddit.com/r/ShitpostXIV/comments/w6vxq3/my_favorite_ffxiv_pastime/>`_.

Sphinx Hints
============

While the `official sphinx documentation <http://www.sphinx-doc.org/en/master/>`__ should be your go-to resource for "how should I do a certain thing in Sphinx," this page offers a list of common features that MRWolf projects will likely need:

Code Blocks
-----------

Code blocks are usually handled with the ``code-block`` directive:

.. code-block:: text

  .. code-block:: java

    System.out.println("Hello World!");

.. code-block:: java

  System.out.println("Hello World!");

Occasionally, it is convenient to sample code multiple code blocks from a single source file.  If the file is included in the project directory, then this can be done with the `literalinclude <https://www.sphinx-doc.org/en/1.5/markup/code.html#Includes>`__ directive.

If the source file is not present in the project directory, but is hosted on the web, the `remoteliteralinclude <https://pypi.org/project/sphinxcontrib-remoteliteralinclude/>`__ extension can be used.  This is included in the default template.

.. TODO:: Can this work with code hosted on private repos?

Tabs
----

Tabbed content can be included by using the ``tabs`` directive (the tabs extension for Sphinx is already included in the project template):

.. code-block:: text

  .. tabs::

    .. tab:: Tab 1

      Here's some tab content!

    .. tab:: Tab 2

      Here's some other tab content!

.. tabs::

  .. tab:: Tab 1

    Here's some tab content!

  .. tab:: Tab 2

    Here's some other tab content!

Admonitions
-----------

Admonitions (such as notes and warnings) are extremely helpful for calling reader attention to important details, and should be used often:

.. code-block:: text

  .. note:: This is a note!

.. note:: This is a note!

The following is a list of available admonitions:

* ``attention``
* ``caution``
* ``danger``
* ``error``
* ``hint``
* ``important``
* ``note``
* ``tip``
* ``warning``

TODOs
-----

Like the code being documented, the documentation itself is a living project.  It will almost never be in a truly "finished" state.  Accordingly, it is useful to be able to mark TODOs for easy review.  This can be done with the ``TODO`` directive:

.. code-block:: text

  .. TODO:: A note on what needs to be done.

By default, TODOs will *not* be displayed in the built documentation, and will only be visible in source.  Their display can be enabled by `changing the appropriate setting <https://www.sphinx-doc.org/en/master/usage/extensions/todo.html>`__ in your project's ``conf.py``.

Sphinx Extensions
-----------------

Occasionally, you'll want to do something not supported by the default features included in this template.  That's OK!  Sphinx is extremely customizeable, and can do most anything you want (with enough effort).

Community-Contributed Sphinx Extensions
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A wealth of community-written, open-source Sphinx extensions can be found at `sphinx-contrib <https://github.com/sphinx-contrib>`__.  Even more can be found on google.

Custom Sphinx Extensions
^^^^^^^^^^^^^^^^^^^^^^^^

In some rare cases, no existing Sphinx extension will serve your purpose.  Thankfully, it is very easy to write a custom Sphinx extension.  For guidance on how to do this, see the `Sphinx extension tutorials <https://www.sphinx-doc.org/en/master/development/tutorials/helloworld.html`__.  As Sphinx is entirely open-source, it is often a good idea to start by modifying one of the existing Sphinx directives.

Getting Started with Sphinx
===========================

This document will guide users through starting a Sphinx documentation project with the MRWolf Sphinx Template.

Official Sphinx Docs
--------------------

In order to use the Sphinx Documentation Template, it's first necessary to familiarize yourself with Sphinx.

Thankfully, Sphinx has extensive documentation; accordingly, users should first skim the official sphinx docs, and keep it on hand as a reference while using the template:

http://www.sphinx-doc.org/en/master/

The official Sphinx documentation will be referred to extensively throughout this guide.

The MRWolf Sphinx Template
--------------------------

The MRWolf Sphinx Template is a baseline Sphinx project set up with the Munich Re company branding and color scheme.  It is the standard foundation that all MRWolf project-level documentation should be based on.

That said, nothing in this template is "set in stone."  Users should not change things haphazardly, as consistency in documentation across projects is extremely important for facilitating readability, but the extremely customizeable nature of Sphinx means that nearly anything can be changed, if desired.  The provided default settings should work for most projects, but are recommendations only.

.. TODO:: Link to template when it has a permanent location.

Starting Your Project from the Template
---------------------------------------

The first step to starting a MRWolf Sphinx Documentation project is to copy the template's git repository into your own documentation project's repository.

Until a permanent hosting solution is found, the template can be found here:

https://github.com/MRWolves/sphinx-template

To create a copy of the documentation template, simply create a new GitHub repository, select "copy from existing source" on the new repo splash page, and entre the template URL.

.. TODO:: finish this section once the template is hosted in a permanent location

Hosting Your Project
--------------------

.. warning:: The temporary hosting solution is *public*.  Do not put any sensitive information on a publicly-hosted Sphinx page!

After the project has been started, it's time to set up hosting - once the hosting process has been configured, your documentation will be automatically built and hosted from your documentation project repository.

Until a permanent hosting solution is found, a temporary solution is to host your project on ReadTheDocs.  Sphinx integration with RTD is simple.  Simply create an account on https://readthedocs.org/, and follow the instructions for hosting documentation from the github repository you set up in the previous step. 

.. TODO:: finish this section once the hosting process is finalized

Configuring CI for Your Project
-------------------------------

.. TODO:: Write this section when CI is worked out.

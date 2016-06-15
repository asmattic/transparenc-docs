Developer
==================

General development specifications for transparenC.

Writing This Documentation
--------------------------

This documentation is maintained in this Github repository `<https://github.com/moldfield/transparenc-docs>`_ . It is written in `reStructuredText <http://sphinx-doc.org/rest.html>`_ using the `Sphinx <http://sphinx-doc.org/>`_ tool that auto generates documentation in html and presents it in the `Read the Docs <http://docs.readthedocs.io/en/latest>`_ theme. 

The `Read the Docs Account <https://readthedocs.org/dashboard/>`_ automatically updates and rebuilds the documentation upon pushing new commits to the Github repository attached to the account. The documentation is built in responsive html, PDF and Epub formats and is available for download in any of the versions that are created over time in multiple languages.



Developing the Codebase
-----------------------

This application is developed as a Wordpress theme and plugin combination located in this private Github repository `<https://github.com/moldfield/transparenc>`_ .

Testing and developing post release versions are done on different branches are to be done on ``test`` and ``post-release`` versions, or specific short-term branches for individual features. In general, the ``master`` branch is used to maintain the ``current-release`` version.

.. note::
	Versioning of this application is done using  `PEP 440`_ spec with
	version numbers like ``1.2.10``.

.. _PEP 440: https://www.python.org/dev/peps/pep-0440/


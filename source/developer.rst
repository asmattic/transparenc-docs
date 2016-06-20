Developer
==================

.. Variables
.. include:: vars.rst

General development specifications for |AppName|_ and the |TestAppName|_.

Developing the Codebase
-----------------------

This application is developed as a Wordpress theme and plugin combination located in this private Github repository `<https://github.com/moldfield/transparenc>`_ .

Testing and developing post release versions are done on different branches are to be done on ``test`` and ``post-release`` versions, or specific short-term branches for individual features. In general, the ``master`` branch is used to maintain the ``current-release`` version.

.. note::
	Versioning of this application is done using  `PEP 440`_ spec with
	version numbers like ``1.2.10``.

.. _PEP 440: https://www.python.org/dev/peps/pep-0440/

Managing Versions
-----------------

Database Transfer
~~~~~~~~~~~~~~~~~~

Common database migration queries.

.. note::
	Make sure to check if the table prefixes are correct.


.. code-block:: sql
	
	UPDATE maa_posts SET post_content = REPLACE(post_content, 'analytics.mckayadvertising.com', 'app.mckayadvertising.com');

	UPDATE maa_posts SET guid = REPLACE(guid, 'analytics.mckayadvertising.com', 'app.mckayadvertising.com');

	UPDATE maa_posts SET post_excerpt = REPLACE(post_excerpt, 'analytics.mckayadvertising.com', 'app.mckayadvertising.com');

	UPDATE maa_options SET option_value = REPLACE(option_value, 'analytics.mckayadvertising.com', 'app.mckayadvertising.com');


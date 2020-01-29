=============================
Django like lookup
=============================

.. image:: https://badge.fury.io/py/django-like-lookup.svg
    :target: https://badge.fury.io/py/django-like-lookup

.. image:: https://travis-ci.org/PetrDlouhy/django-like-lookup.svg?branch=master
    :target: https://travis-ci.org/PetrDlouhy/django-like-lookup

.. image:: https://codecov.io/gh/PetrDlouhy/django-like-lookup/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/PetrDlouhy/django-like-lookup

PostgreSQL LIKE lookup functionality for Django. Django does contain __startswith, __endswith and __contains lookups, but all of them does escape "%" and "_" wildcard characters. The `__like` lookup is often faster, than the `__regex` lookup, so it can be used in cases when conditions are simple enough.

Documentation
-------------

The full documentation is at https://django-like-lookup.readthedocs.io.

Quickstart
----------

Install Django like lookup::

    pip install django-like-lookup

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'like_lookup.apps.LikeLookupConfig',
        ...
    )

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage

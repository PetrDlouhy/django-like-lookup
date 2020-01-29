=====
Usage
=====

To use Django like lookup in a project, add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'like_lookup.apps.LikeLookupConfig',
        ...
    )

Add Django like lookup's URL patterns:

.. code-block:: python

    from like_lookup import urls as like_lookup_urls


    urlpatterns = [
        ...
        url(r'^', include(like_lookup_urls)),
        ...
    ]

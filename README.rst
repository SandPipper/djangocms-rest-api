===================
djangocms-rest-api
===================

An application to use CMS content and features via REST API.

djangocms-rest-api uses Django REST framework to serve django CMS data through a REST API

Installation
------------

* git clone https://github.com/SandPipper/djangocms-rest-api
* add djangocms_rest_api folder to your project
* pip install beautifulsoup4
* Edit ``INSTALLED_APPS``::

    INSTALLED_APPS = [
        ...
        'rest_framework',
        'djangocms_rest_api',
        ...
    ]

* Edit ``urls.py``::

    urlpatterns = [
        ...
        url(r'^api/', include('djangocms_rest_api.urls', namespace='api')),
        ...
    ]

* api/pages/ - to fetch all pages with their placeholders and plugins
* api/contents/ - to fetch header and footer

* That's all!


Features
--------


Credits
-------


License
-------

MIT

=============
ckanext-datagovro_theme v2
=============

.. image:: https://travis-ci.org/john21ro/ckanext-datagovro_theme.svg?branch=master
    :target: https://travis-ci.org/john21ro/ckanext-datagovro_theme

This extensions includes the custom theme plugin used by 
http://data.gov.ro/ .


------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-datagovro_theme:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Clone ckanext-datagovro_theme repo and cd into directory

3. Install the ckanext-datagovro_theme Python package into your virtual environment::

     python setup.py develop

3. Add ``datagovro_theme`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------

```
datagovro_theme.custom_resource_download_url = http://data.gov.ro
datagovro_theme.google_analytics_token_path = /etc/ckan/default/google-analytics-secrets.json
```

-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini

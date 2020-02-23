=================================
Welcome to django-admin-csvexport
=================================

Description
===========
Django-admin-csvexport is a django-admin-action, that allows you to export a
selection of the fields of your models as csv-formatted data.

Features
========
* selectable model-fields
* inclusive of related models
* customizable csv-format
* view or download csv-data

Django
======
csvformat was developed with django-2.2. Probably it works with other
django-versions (1.11 to 2.2).

Installation
============
Install from pypi.org::

    pip install django-admin-csvexport

Add csvexport to your installed apps::

    INSTALLED_APPS = [
        'csvexport',
        ...
    ]

Add csvexport to the actions of your modeladmin::

    from csvexport.actions import csvexport

    class MyModelAdmin(admin.ModelAdmin):
        ...
        actions = [csvexport]

Todo
====
* Implement a test-suite and setup continuous integration with travis.
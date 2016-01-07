# Python Status.io 

A Python wrapper around the Status.io API.

[![Downloads](https://img.shields.io/pypi/v/python-statusio.svg)](https://pypi.python.org/pypi/python-statusio/)
[![Travis CI](https://travis-ci.org/statusio/python-statusio.svg)](https://travis-ci.org/statusio/python-statusio)

## Introduction

This library provides a pure Python interface for the [Status.io API](http://docs.statusio.apiary.io/). It works with Python versions from 2.6+.

[Status.io](http://status.io) provides hosted system status pages.

## Installing

You can install python-statusio using::

    $ pip install python-statusio

## Documentation

View the last release API documentation at: http://developers.status.io/

## Using

The library provides a Python wrapper around the Status.io API.

### API

The API is exposed via the `statusio.Api` class.

To create an instance of the `statusio.Api` with yout credentials:

    >>> import statusio
    >>> api = statusio.Api(api_id='api_id',
                          api_key='api_key')

To your status page summary:

    >>> summary = api.StatusSummary('status_page_id')
    >>> print(summary)

There are many more API methods, to read the full API documentation::

    $ pydoc statusio.Api
# Bitfinex Python Client

A Python client for the Bitfinex API.

Most of the unauthenticated calls have been implemented.  It is planned to
implement the remainder of the API.


## Setup

Install the libs

    pip install -r ./requirements.txt


## Tests

Depending on your system, install one of the following libs

- pyinotify (Linux)
- pywin32 (Windows)
- MacFSEvents (OSX)

Sniffer will watch for changes

    sniffer -x --nocapture

Or Sniffer with code coverage enabled...

    sniffer -x --nocapture -x--with-coverage -x--cover-html -x--cover-package=bitfinex

Or you can just run the tests

    nosetests

### Test Coverage

Test coverage of the code. View cover/index.html to view detailed reports.

    nosetests --with-coverage --cover-html --cover-package bitfinex


## Usage

See the examples directory for samples.

e.g.

    PYTHONPATH=.:$PYTHONPATH python examples/basic.py


## Compatibility

This code has been tested on

- Python 2.7.5
- Python 3.3.1


## TODO

- Package the code so it can be installed by pip.
- Implement all API calls.


## References

- [https://www.bitfinex.com/pages/api](https://www.bitfinex.com/pages/api)


## Licence

The MIT License (MIT)

Copyright (c) 2014 Scott Barr

See [LICENSE.md](LICENSE.md)

GLADYS
======

*The Graph Library for Autonomous and DYnamic Systems* [![Build Status]
(https://travis-ci.org/pierriko/gladys.png?branch=master)](https://travis-ci.org/pierriko/gladys)

Concept
-------

Provide an API for high level robotic planners from Georeferenced data.

.. code::

    +------+    +--------+    +-----+
    |      |    |        |    |     |
    | GDAL |--->| gladys |--->| BGL |
    |      |    |        |    |     |
    +------+    +--------+    +-----+
                    ^
                    |
                /~~~~~~~~~~\
                /            \
                | Wild World |
                \            /
                \~~~~~~~~~~/


Links
-----

* http://gdal.org
* http://boost.org/libs/graph
* http://www.openrobots.org/wiki
* http://trac.laas.fr/git/gladys


HOWTO
-----

.. code::

    git clone http://trac.laas.fr/git/gladys && cd gladys
    mkdir build && cd build
    cmake -DCMAKE_INSTALL_PREFIX=$HOME/devel ..
    make -j8 && make test && make install
    # for verbose test:
    ./test/test_gladys --log_level=test_suite


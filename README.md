FakeCoin : A totaly Real Crypto
===============================

https://www.reddit.com/r/FakeCoin/

Copyright (c) 2009-2013 Bitcoin Developers |
Copyright (c) 2011-2013 Litecoin Developers |
Copyright (c) 2017-2018 Diamond Group

FakeCoin is Secure, safe, and fast.

But most of all: FakeCoin is REAL.

What is FakeCoin?
=================

FakeCoin, the brainchild of Scynetoshi Blackamoto, is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 2.5 minute block targets
 - subsidy halves in 840k blocks (~4 years)
 - ~84 million total FAKs (Pronounced "fAuk")

The rest is the same as Bitcoin except better.
 - 50 FAKs per block
 - 2016 blocks to retarget difficulty

For more information, as well as an immediately useable, binary version of
the FakeCoin client sofware, visit https://www.reddit.com/r/FakeCoin/.

License
-------

Diamond Group beleaves that FakeCoin will benefit all of mankind and so it is released under the terms of the MIT license. See `COPYING` for more

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the FakeCoin
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion (if they haven't already) on the
[Subreddit](https://www.reddit.com/r/FakeCoin/).

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch has been built and tested, but is not guaranteed to be
completely stable.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test FakeCoin-qt.pro
    make -f Makefile.test
    ./fakecoin-qt_test

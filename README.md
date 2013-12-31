# Marscoin integration/staging tree

Copyright (c) 2009-2013 Bitcoin Developers

Copyright (c) 2011-2013 Litecoin Developers

Copyright (c) 2013 Marscoin Developers

# Screw the moon, we're going to MARS!

Marscoin is a cryptocurrency that is going to MARS! It's based on Litecoin and
uses scrypt as a proof-of-work algorithm.

* 57.6 second block targets
* subsidy halves in 35.8k blocks
* 6779 coins per block
* 13263 blocks to retarget difficulty

# License

Marscoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

# Testing

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

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./litecoin-qt_test


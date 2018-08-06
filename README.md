Kennedycoin integration/staging tree
================================

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2018 Kennedycoin Developers

What is Kennedycoin? KENN
----------------

Kennedycoin (KENN) is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.

 - Algorithm Scrypt
 - Type	PoW
 - RPC port	3377
 - P2P port 3378
 - Block reward 50 coins
 - Block halving 210k blocks
 - Coin supply	27,300,000 coins
 - Coinbase maturity 10 blocks
 - Target spacing  2 minutes
 - Target timespan	10 minutes
 - Transaction confirmations 9 blocks

Windows Wallet
----------------
https://github.com/lgncoin/Kennedycoin/blob/master/Kennedycoin-qt-windows.zip

you can mining solo by wallet By writing (setgenerate)

Go to Help & Click Debug Window & Console Then Type : setgenerate

Linux Wallet
----------------
https://github.com/lgncoin/Kennedycoin/blob/master/Kennedycoin-qt-linux.tar.gz

You need to install the following dependencies to start your wallet in Ubuntu desktop

sudo apt-get install build-essential libssl-dev libdb-dev libdb++-dev libboost-all-dev git libssl1.0.0 libdb-dev libdb++-dev libminiupnpc-dev libevent-dev libcrypto++-dev libgmp3-dev libqt5widgets5

*Seednode
---------
addnode 159.89.146.14 add

addnode 217.182.170.20 add

addnode 92.222.36.221 add

--------------------------------------------------------------------------------

License
-------

Kennedycoin is released under the terms of the MIT license. 
See `COPYING` for more
information or see http://opensource.org/licenses/MIT.


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

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./Kennedycoin-qt_test


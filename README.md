


# **Hexxcoin [HXX] swap 2017**

Anonymous Zerocoin Protocol:
https://en.wikipedia.org/wiki/Zerocoin

Zerocoin  parameters RSA-2048 from RSA Factoring Challenge
https://en.wikipedia.org/wiki/RSA_Factoring_Challenge

Hexxcoin
----------------
* Coin Suffix: HXX
* Algorithm:lyra2rev2 from Zoin(not Zcoin)
* Algo params: LYRA2(BEGIN(thash), 32, BEGIN(nVersion), 80, BEGIN(nVersion), 80, 2, 330, 256)
* Target Spacing: 150 Seconds
* Retarget: every block
* Reward per Block: 
	There will be a slow start, 4 weeks / 1 coin.
	Then 2 weeks / 25 coins.
	6 weeks / 12.5 coins
	6 weeks / 6.25 coins
	6 weeks / 3.125 coins
	6 weeks / 1.5625 coins
	And finally, 1 coin reward / block
* Confirmation: 6 Blocks
* Maturity: 120 Blocks
* Blocks: ~576 per day
* Total Coins: 9,999,999 HXX
* Min TX Fee: 0.0001 HXX
* Block Size: 4MB


**Net Parameters**
P2P Port = 29100
RPC Port = 29200
Client core = 0.8.7
Clien name = hexx.exe
Conf file = hexx.conf

Installation folder :
Windows: C:\Users\Username\AppData\Roaming\hexx
Mac:/Library/Application Support/hexx
Unix: /.hexx




Debian/Ubuntu Linux Daemon Build Instructions
================================================

install dependencies:

    $ sudo apt-get update && sudo apt-get upgrade
    $ sudo apt-get install git build-essential libssl-dev libdb5.3++-dev libminiupnpc-dev libboost-all-dev

build hexxd from git:

    $ git clone https://github.com/hexxcointakeover/hexxcoin
    $ cd hexxcoin/src && make -f makefile.unix
   
install and run hexxd daemon:

    $ sudo strip hexxkd && sudo cp ~/hexxcoin/src/dd /usr/bin && cd ~/
    $ hexxd

here are a few commands, google for more.

    $ ./hexxd getinfo
    $ ./hexxd getpeerinfo
    $ ./hexxd getmininginfo
    $ ./hexxd getnewaddresss
	

Debian/Ubuntu Linux Qt4 Wallet Build Instructions
================================================

update and install dependencies:

    $ sudo apt-get update && sudo apt-get upgrade
    $ sudo apt-get install git build-essential libssl-dev libdb5.3++-dev libminiupnpc-dev libboost-all-dev qt4-qmake libqt4-dev
build Hexxcoin-qt from git:

    $ git clone clone https://github.com/hexxcointakeover/hexxcoin
    $ cd hexxcoin && qmake -qt=qt4 "RELEASE=1" Hexxcoin-qt.pro && make
 
running the Hexx Qt wallet:

    $ sudo ./hexx
 
 Debian/Ubuntu Linux Qt5 Wallet Build Instructions
================================================

update and install dependencies:

    $ sudo apt-get update && sudo apt-get upgrade
    $ sudo apt-get install git build-essential libssl-dev libdb5.3++-dev libminiupnpc-dev libboost-all-dev qt5-qmake libqt5gui5 libqt5core5 libqt5dbus5 qttools5-dev-tools
build Hexxcoin-qt from git:

    $ git clone clone https://github.com/hexxcointakeover/hexxcoin
    $ cd hexxcoin && qmake -qt=qt5 "RELEASE=1" Hexxcoin-qt.pro && make
 
running the Hexx Qt wallet:

    $ sudo ./hexx

Example hexx.conf Configuration
===================================================

	rpcallowip=127.0.0.1
	rpcuser=MAKEUPYOUROWNUSERNAME
	rpcpassword=MAKEUPYOUROWNPASSWORD
	rpcport=29100
	server=1
	listen=1
	port=29200



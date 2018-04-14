# CarrotBinaries Linux Download Instructions

Download and copy binaries to desired folder

##Ubuntu 16.04 and 17.04

1 -- Update your apt cache
 
`ubuntu@server:~$ sudo apt-get update` 

2 -- Install the carrot dependencies

`ubuntu@server:~$ sudo apt-get -y install libevent-dev libboost-all-dev libminiupnpc10 libzmq5 software-properties-common`

3 -- You need version 4 of the BerkeleyDB, the easiest way is to use the bitcoin apt packages, add the bitcoin repository 

`ubuntu@server:~$ sudo add-apt-repository ppa:bitcoin/bitcoin`

4 -- Update your apt cache to recognize the new bitcoin repository

`ubuntu@server:~$ sudo apt-get update`

5 -- Install the BerkeleyDB4 dependency

`ubuntu@server:~$ sudo apt-get -y install libdb4.8-dev libdb4.8++-dev`

6a -- If you want to run the carrotd binary

`ubuntu@server:~$ ./carrotd -daemon`

6b -- If you want to run the GUI carrot-qt binary you will need to add an addtional library before starting

`ubuntu@server:~$ sudo apt install libqrencode3`

`ubuntu@server:~$ ./carrot-qt`

##CentOS

1 -- Add the EPEL repository

`root@server:~# yum -y install https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm`

2 -- Install the carrot dependencies

`root@server:~# yum -y install zeromq libevent boost libdb4-cxx miniupnpc`

3 -- Start carrotd

`root@server:~# ./carrotd -daemon`

##Fedora

1 -- Install the carrot dependencies

`root@server:~# yum -y install zeromq libevent boost libdb4-cxx miniupnpc`

2 -- Start carrotd

`root@server:~# ./carrotd -daemon`





Custom LEDE Patch For TL-WR1043ND
======================================================

Dependencies
------------

* LEDE BuildRoot
* LEDE BuildRoot Dependencies
* Java Runtime

How to use
----------

* Install all the development packages required for LEDE BuildRoot
* Install Java Runtime
* Clone the LEDE Repository

    git clone -b lede-17.01 https://github.com/lede-project/source.git lede

Clone this Repository and copy into the LEDE repository

    git clone -b lede-17.01 https://github.com/gwlim/mips24k-lede-patch.git temp; mv temp/* lede/; rm -rf temp

Change directory into the LEDE Repository

    cd lede

Run the script

./patch_LEDE.sh

Make Menuconfig Default Target Profile is TP-LINK TL-WR1043ND (all the packages and config is inside)

    make menuconfig

Save and make

    make V=s

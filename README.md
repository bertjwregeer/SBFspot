SBFspot is an open source project to get actual and archive data out of an SMA
inverter over bluetooth. It should work on either Linux and Windows.

This is a Github mirror of the Codeplex repository: https://sbfspot.codeplex.com/

# Installation

    apt-get install git bluetooth libbluetooth-dev libboost-all-dev build-essential
    git clone $THISREPO
    cd SBFSpot
    make release

Alternate releases are also available:

## sqlite3:

    apt-get install sqlite3-dev libsqlite3-dev
    make release_sqlite

## MySQL:

    apt-get install libmysqlclient-dev`
    make release_mysql`

# Usage

 - `hcitool scan` to find the Bluetooth address of the SMA inverter
 - Modify the `SBFspot.cfg` file with the appropriate settings
 - `./bin/Release/SBFspot -cfg./SBFspot.cfg`

.. _bloqstarted:

Getting Started
===============

This section provides the information to quickly get up to speed and start building applications on top of the Bloq ecosystem.

First step
----------
Get acquainted with Fabric composer, which allows developers to define business networks that can be deployed on a Hyperledger Fabric instance.
See `Hyperledger composer <https://github.com/fabric-composer/fabric-composer>`__ for more information.

BloqNetwork codebase
--------------------
The code is available on `Github <https://github.com/notarynodes/composer/tree/master/bloqNetwork>`__.

Fabric instance
---------------
The Bloqs Business network is deployed on NotaryNodesV1 which runs on Bluemix.
Composer-connection-profile information will be shared soon for both the test and production network.

Test data
~~~~~~~~~
Soon information will be released on how to connect to the test network that holds Mainstreet 1 Bloq data.

Production data
~~~~~~~~~~~~~~~
Summer 2017 Bloqhouse will launch a pilot with *real* real estate. After asset emission and bloqification Bloq data will become available to the development community.

.. _bloqapi:

API specification
-----------------

.. warning:: The API is still subject to continuous changes and updates will probably not be backwards compatible.

Transaction functions
---------------------

* /CreateFund input: {transactionId, creator, signer, fundId, properties}
* /Sign input: {transactionId, signer, assetType, assetId}
* /BloqEmission input: {transactionId, fund, signer, escrow, count}
* /BloqTransfer input: {transactionId, origin, destinations, counts}
* /GetHolderBloqcounts input: {transactionId, holder}

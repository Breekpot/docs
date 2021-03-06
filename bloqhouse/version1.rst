NotaryNodes V0.1
================

.. note:: The NotaryNodes initiative is technology agnostic.

The first proof-of-concept we've built on top of the Hyperledger Fabric protocol.
Assets (chaincode) were created using Fabric composer, a tool that allows developers to easily define assets and business networks in client-side javascript.

To read more about the first asset, see :ref:`bloqintro`.

* `Hyperledger fabric <https://hyperledger-fabric.readthedocs.io/en/latest>`__
* `Fabric composer <https://fabric-composer.github.io>`__

.. _fabricimplementation:

Hyperledger fabric
------------------

NotaryNodes v0.1 is a hosted instance of the fabric protocol. Integrity of protocol execution (hosting peers) is safeguarded by notaries.
Its optimized for use cases that involve regulated assets. E.g. it will provide re-useable functionality to connect to official identity providers such as idensys.

V0.1 is a *general purpose* permissioned ledger.

.. figure:: ../images/notarynodes.png
    :scale: 70 %
    :alt: NotaryNodes
    :align: center

    NotaryNodes

    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/notary.png         | (Dutch) notary        | .. image:: ../images/node.png           | Network node / peer   |
    |    :width: 30px                         |                       |    :width: 30px                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+

|

We are investigating the setup that allows notaries to safeguard integrity of protocol execution.
Any officially registered notary should be able to join the initiative, so that market forces keep transaction costs at a fair price point.

Among many other questions we are currently investigating, through workshops, what the exact role of the notary will be.

Identity management
~~~~~~~~~~~~~~~~~~~

To create digital representations of regulated assets *know your customer* (KYC) functionality has to be implemented.
Any serious solution will also require strong mechanisms to safeguard privacy.

A first solution that integrates a trusted identity provider iDIN with the Hyperledger Fabric CA was built by IBM, Van Doorne and Bloqhouse during the Dutch Blockchain Hackathon.

External sources
~~~~~~~~~~~~~~~~

* `Mr-online article idintt solution <http://www.mr-online.nl/doorne-als-enige-op-blockchain-event>`__
* `Idintt hackathon contribution, the codebase <https://github.com/notarynodes/idintt>`__
* `Dutch Blockchain Hackathon <https://blockchainhackathon.eu>`__

(Enterprise) Ethereum
---------------------

More information will soon follow.

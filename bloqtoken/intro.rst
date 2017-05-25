.. _bloqintro:

What is a Bloq?
===============

A Bloq is a digitized ownership certificate of a legal entity holding a real estate object.
It entitles the owner to the economic benefits realized by the entity (direct profit / monthly rent).
In case of an increase in value of the underlying property the holder of a Bloq will also make a profit when he/she sells the Bloq (indirect profit).
Bloq value is determined by the demand and supply market.
The below image visualizes the entities involved.

|

.. figure:: ../images/overview.png
    :scale: 50 %
    :alt: Overview of entities
    :align: center

    Overview of entities

    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/property.png       | Property              | .. image:: ../images/assetmanager.png   | Fund manager          |
    |    :width: 30px                         |                       |    :width: 30px                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/business.png       | Legal entity / fund   | .. image:: ../images/crowd.png          | Crowd                 |
    |    :width: 30px                         |                       |    :width: 30px                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/legalowner.png     | Legal ownership       | .. image:: ../images/tenant.png         | Tenant                |
    |    :width: 30px                         |                       |    :width: 30px                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/bloq.png           | Bloq                  |                                         |                       |
    |    :width: 30px                         |                       |                                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+

|

Characteristics of a Bloq:
  * It's a digital representation of a (partial) economic ownership certificate
  * Bloqs entitle holders to the profits being made, it doesn't give them voting rights
  * Bloqs holders are not liable for a potential loss
  * Bloqs are fungible
  * Bloqs can be traded directly peer-to-peer without notary approval
  * Bloq holders should always be identifiable to prevent money laundering

|

Digitized asset
---------------

Currently it's common practice for private real estate funds to issue certificates that do not have a (standardized) digital representation.
Bloqification will replace offline (sometimes physical) shareholder registers with digital smart contracts hosted on blockchain technology.

Per business entity a smart contract is written and deployed. Within the smart contract's inner database the names of shareholders are stored.
Regulation of financial markets requires Bloq holders to be identifiable. Bloqholder names are encrypted.

Users can make calls (via software) to smart contract functions to transfer Bloqs. Certain calls such as updating the fund manager require a crypto signature by a registered notary.
See the :ref:`bloqapi` for an overview of the implemented methods.

|

.. figure:: ../images/smart_contract.png
    :scale: 50 %
    :alt: Property smart contract
    :align: center

    Property smart contract

|

.. figure:: ../images/architecture.png
    :scale: 50 %
    :alt: Architecture
    :align: center

    Architecture

|

Regulation
----------

Real estate is regulated, as is trading in financial instruments. We involve **regulators** from the beginning to design solutions **collaboratively**.
Relevant regulators and institutions are the Financial Markets Authority (AFM), Tax department, Dutch bank (DNB) and European central bank (ECB).

Permissioning
~~~~~~~~~~~~~

.. note:: Please read the section about :ref:`codemeetslaw` first.

Which blockchain to use? And in case of permissioned blockchains who will control the peers?

The most disintermediating option, except for permissionless solutions, would be to have the fund managers (creators of the smart contracts) setup a peer network themselves.
An advantage is that the fund manager needs to be trusted by the bloqholders anyway. This option would effectively eliminate the need for any other trusted middle men such as exchanges (e.g. Euronext) and brokers.

We foresee that traditional exchanges and broker services will be replaced by more value added services that have to be very price efficient as they operate without a monopoly / authority.
An example service on top of the Bloq ecosystem is the :ref:`bloqhouse`, which provides:

* Bloqholder convenience and UX
* Fiat currency exchange (eliminate real world friction)
* A platform; connecting Bloqholders

NotaryNodes
~~~~~~~~~~~

Instead of fund managers controlling the peers. NotaryNodes is working on a different scenario; where a network of notaries control the network of peers.
The notary is a middle men that, by law, is already part of the chain of trust (notaries approve Bloq emmissions etc.).

We believe that instead of having many specialized permissioned blockchains; e.g. one for real estate ran by fund managers and one for book vouchers ran by bookstores.
It makes sense to profit from economies of scale; a general purpose permissioned blockchain where notaries guarantee integrity of protocol execution by controlling the nodes.

We believe economies of scale will result in quality and expertise at a lower price. To guarantee quality at a fair price, it's important to allow competition.
That is why NotaryNodes is an open initiative that allows any registered notary to join.

We are working on a pilot version that hosts the Bloq ecostem on NotaryNodes v1.

The permissionless option
~~~~~~~~~~~~~~~~~~~~~~~~~

The goal is not to use blockchain technology, which for some is equal to permissionless solutions. The goal is to create a digital real estate ownership ecoystem that accelerates innovation.
Both a permissionless and permissioned option provide many benefits to the current systems:

* it increases standardization of digital representations of assets
* the system is transparent
* there is no single exchange with a trading monopoly
* smart contract business logic can store mechanisms to manage identities and prevent money laundering

We believe those improvements will have a big positive impact on scaling the Bloq ecosystem and foster innovation.

See the section about :ref:`codemeetslaw` that discusses difficulties with a permissionless setup including:

* updates to smart contract business logic in case of regulation changes
* forks and bugs
* protocol leadership
* risks related to an anonymous mining community

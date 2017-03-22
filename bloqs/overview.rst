.. _bloqintro:

What is a Bloq
==============

A bloq is a digitized ownership certificate of an legal entity holding a real estate object.
It entitles the owner to all economic benefits coming out the legal entity. This includes the monthly rent and, if applicable, the increase in property value.
The below image explains the entities involved.

|

.. figure:: ../images/overview.png
    :scale: 50 %
    :alt: Overview of entities
    :align: center

    Overview of entities

    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/property.png       | Property              | .. image:: ../images/assetmanager.png   | Asset manager         |
    |    :width: 30px                         |                       |    :width: 30px                         |                       |
    +-----------------------------------------+-----------------------+-----------------------------------------+-----------------------+
    | .. image:: ../images/business.png       | Business entity       | .. image:: ../images/crowd.png          | Crowd                 |
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
  * It's a digital representation of a certificate
  * The certificate is a proof of partial economic, non-voting, ownership
  * Bloqs are fungible
  * Bloqs are tradable peer-to-peer without notary involvement
  * Bloq holders should be identifiable to prevent money laundering
  * Bloq holders are entitled to their share of the monthly rent (after costs)

|

Digitized asset
---------------

Currently its common practice for private real estate funds to issue certificates that do not have a (standardized) digital representation.
Bloqification will replace offline (sometimes physical) shareholder registers with digital cloud-hosted smart contracts.

Per business entity a smart contract is written and deployed. Within the smart contract's inner database the names of shareholders are stored.
Regulation of financial markets requires Bloq holders to be identifiable. Bloqholder names are encrypted such that it requires two keys to decrypt them.
The asset manager will hold one of them, the other is in the possession of regulators.

Developers can call smart contract functions to transfer bloqs or change the asset owner (which requires a crypto signature by a notary).
See the :ref:`bloqapi` for an overview of the implemented methods.

|

.. figure:: ../images/smart_contract.png
    :scale: 50 %
    :alt: Property smart contract
    :align: center

    Property smart contract

|

Legal
-----

We involve regulators from the beginning to design solutions collaboratively.
Relevant regulators and institutions are Financial Markets Authority (AFM), Tax department, Dutch bank (DNB) and European central bank (ECB).

De-central?
~~~~~~~~~~~

The goal is not to use blockchain technology. The goal is to create a digital real estate ownership ecoystem that accelerates innovation.

Bloq smart contracts are hosted on NotaryNodes V0.1 (:ref:`fabricimplementation`). Which aims to find a sweet spot between public and private blockchains.

Controlled access to update smart contract business logic is facilitated in case  regulation changes, a bug is found or in case the community behind the underlying protocol abandons the project.

The solution we are investigating is to capture, together with a notary and before deployment, the conditions that would allow updates to the code.
Such a solution would trade code-is-law and de-centrality for flexibility in case of necessary change, as that is the only constant we know.

The implications are quite fundamental, for some it undermines the purpose of blockchain technology.
Though we argue that important improvements over the old solutions still hold:

* it increases standardization of digital representations of assets
* the system is transparent
* there is no trading house with a trading monopoly
* smart contract logic lowers trading friction
* smart contract logic can hold mechanisms to manage identities and prevent money laundering

We believe those improvements will have a big positive impact on scaling the Bloq ecosystem and foster innovation.

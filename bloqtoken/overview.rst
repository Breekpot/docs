.. _bloqintro:

The BloqToken
=============

.. note:: This is a work in progress.

Tokenized investment funds
--------------------------
The first tokenized assets (BLT) will be real estate investment funds managed by AIFMd registered Alternative Investment Fund Managers.
For every legal entity (a fund) holding one or more real estate objects an ERC20 BloqToken is deployed to Ethereum.
Bloqtokens are digital representations of economic fund ownership certificates. By representing them digitally we make them inherently p2p tradeable.

The real estate object(s) owned by the fund are rented to one or more tenants.
As a Bloqtoken owner you're entitled to the economic benefits realized by the entity. The direct profit is equal to the rent minus management costs.
On the secondary market Bloqs can be traded peer-to-peer, Bloqholders can thus make an indirect profit from value appreciation of the underlying assets (real estate).
Bloq value is determined by the market; demand and supply.

Characteristics of a Bloq:
  * It's a digital representation of a (partial) economic ownership certificate
  * Bloqs entitle holders to the profits being made, it doesn't provide voting rights for day to day decisions (e.g. deciding about tenants)
  * Bloqsholders are not liable for potential losses
  * Bloqs are fungible
  * Bloqs can be traded directly peer-to-peer without notary approval
  * Bloqholders are anonymous to the public, only the fund manager has access to the identity information of Bloqholders

Regulation
----------
Real estate transactions are regulated, as is trading in financial instruments. We involve **regulators** from the beginning to design solutions **collaboratively**.
Relevant regulators and institutions are the Financial Markets Authority (AFM), Tax department, Dutch bank (DNB) and European central bank (ECB).

BLT Smart contract
------------------
The BloqToken smart contract inherits the `ERC20 <https://theethereum.wiki/w/index.php/ERC20_Token_Standard>`__  token standard contract.
We rely on standards and keep contracts as simple as possible.
The ERC20 standard transfer and transferFrom functions implement an extra condition contract *transferConditions* that performs regulatory compliance checks.
Such as checking the whitelist status (KYC) and adhering to daily trading limits.

For whitelisting the BLT contract relies on oracles / identity service providers.

The token contract is owned/deployed by the Investment fund manager. It's the fund manager who has authority in case of forks, protocol or contract bugs.

Investment documentation
------------------------
Investment documents, such as the prospectus, will be stored on IPF. A link to the IPFS hash is stored within the BloqToken contract.

.. _bloqstarted:

Getting started
---------------
Soon test BLTs will be deployed to the Ropsten testnet.
Contact hello@bloq.house for more information.

.. _bloqathon:

Bloqathon
---------
Q4 2017 Bloqhouse will organize a Bloqathon to kick-start development on top of the **open** Bloqtoken ecoystem.

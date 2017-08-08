.. _bloqintro:

The BloqToken
=============

.. note:: This is a work in progress.

Tokenized investment funds
--------------------------
The first tokenized assets (BLT) will be real estate investment funds managed by AIFMd registered Alternative Investment Fund Managers.
For every legal entity (a fund) holding one or more real estate objects an ERC20 dividend-bearing BloqToken is deployed to Ethereum.
Bloqtokens are digital representations of partial economic fund ownership. Their digital representation enables investor to exchange them with others fully peer-to-peer.

The real estate object(s) owned by the fund are rented to one or more tenants.
As a Bloqtoken owner you're entitled to the economic benefits realized by the entity. The direct profit is equal to the rent minus management costs.
On the secondary market Bloqs can be traded peer-to-peer, Bloqholders can make an indirect profit from value appreciation of the underlying assets (real estate).
Bloq value is determined by demand and supply.

Characteristics of a Bloq:
  * It's a digital representation of a (partial) economic ownership certificate
  * Bloqs entitle holders to the profits (rental income) being made, it doesn't include the power to vote about day-to-day operations
  * Bloqsholders are not liable for potential losses
  * Bloqs are fungible
  * Bloqs can be traded directly peer-to-peer without notary approval
  * Bloqholders are anonymous to the public, only the fund manager has access to the identity information behind public keys

Regulation
----------
Real estate transactions are regulated, as is trading in financial instruments. We involve **regulators** from the beginning to design solutions **collaboratively**.
Relevant regulators and institutions are the Financial Markets Authority (AFM), Tax department, Dutch bank (DNB) and European central bank (ECB).

BLT Smart contract
------------------
The BloqToken smart contract inherits the `ERC20 <https://theethereum.wiki/w/index.php/ERC20_Token_Standard>`__  token standard contract.
The ERC20 standard transfer and transferFrom functions are extended with modifiers that check against extra conditions that ensure regulatory compliance.
Such as checking the whitelist status (know-your-customer).
For whitelisting the contract relies on oracles / identity service providers.

The token contract is owned & deployed by the Investment fund manager. It's the fund manager who has authority in case of forks, protocol or contract bugs.

Investment documentation
------------------------
Investment documents, such as the prospectus, will be stored on IPFS. A link to the IPFS path is stored within the BloqToken contract.

.. _bloqstarted:

Getting started
---------------
Bloqtokens are deployed to Rinkeby testnet for testing purposes. Soon the underlying code will be made available open source on Github.
* Property 1 - 0xD91d5C54f929366d79F282510062E0811fA5600F
* Property 2 - 0x67a87D372f450776Af4D76E0D09374e012012011
* Property 3 - 0x2d9b07C7D2cfFe7A99ED757acE95e8C7eB0CE093
Contact hello@bloq.house for more information.

.. _bloqathon:

Bloqathon
---------
Bloqhouse plans to organize a Bloqathon together with the Blockchain Real Estate Association to kick-start further development on top of the **open** Bloqtoken ecoystem.

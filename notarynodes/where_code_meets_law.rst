Where code meets law
====================

.. note:: This is a work *in progress*. Documentation, legal framework and code all have incubation status. Insights & solutions are subject to constant change!

Why are there relatively few successful applications of blockchain technology to real world problems?

* Code is law is problematic (e.g. the DAO hack)
* Many business models include middle men, blockchain makes them obsolete
* Technology immaturity and uncertainty about new phenomena such as forks
* Trusting a de-central, anonymous, group of miners and developers is not always an option
* Law and regulation still need to catch up

NotaryNodes aims to:

* Apply blockchain to real-world applications (including regulated assets)
* Learn by doing (small scale proof-of-concepts)
* Collaborate with partners such as notaries and technology companies
* Identify new business models and opportunities for partners
* Relax some blockchain principles and make a shift from code is law towards *code meets law*

Code is law
-----------

If it would be that simple, why did we have judges over the past centuries?

+----------------+------------------+------------------------------------+----------------------+
| Contract       | Natural language | Interpreted by judges              | Non-deterministic    |
+----------------+------------------+------------------------------------+----------------------+
| Smart contract | Programming code | Interpreted by a software protocol | Deterministic [#f1]_ |
+----------------+------------------+------------------------------------+----------------------+

.. [#f1] Under a certain protocol.

The past has learned us that interpretation of complex agreements quickly becomes non-deterministic.
Even rather simple agreements such as the DAO code result in different interpretations (ETH vs ETC).

Challenges with code is law
~~~~~~~~~~~~~~~~~~~~~~~~~~~

* Isn't true objective (deterministic) interpretation of complex contracts an utopia?
* Isn't bug-free software an utopia?
* Rapid innovation requires updates to code and the interpreting protocol, how to accommodate for flexibility?

.. _codeislawsolution:

A possible solution
~~~~~~~~~~~~~~~~~~~

The option we are investigating is to rely on a role that provided trust in society for a long time.
The idea is to let a notary hold a cryptographic key that allows updates to the code.

.. note:: Open question: What are the conditions under which the key is released and to who is it released? Who interprets the conditions?

Chain of trust
--------------

Sometimes blockchain networks are called trust-less networks.
The fact that there is no absolute authority does not mean there are no people in the chain of trust.
Behind every piece of software (protocol level and instance level) there is a person:

* The protocol development community and it's leaders
* Smart contract developer
* The miners (or owners of mining farms)

To apply blockchain technology on scale to for example society's pension money; we still need a lot more clarity about the implications of trusting these de-centrally organized, and often anonymous, people.

.. _publicvsprivate:

Public blockchains
------------------

For sure Bitcoin protocol has the most mining power backing it up.
All that mining power creates a high trust level as it makes manipulation of the ledger expensive (on the other hand it makes transactions rather expensive too..).

Given the current maturity of the technology we still see a lot challenges to apply public ledger technology to regulated assets:

* Technological immaturity
* Implications of phenomena such as forks are unclear
* How to account for change? Protocols, languages, hardware but also regulation are subject to constant change. You need strong leadership to change direction, does strong leadership undermine de-centrality?
* Who are you trusting? See the previous section.
* Coin volatility
* Scalability and environmental impact if we further scale
* Large scale tax evasion and it's impact on society if we further scale

That's quite a list of questions if you want to go live with your application tomorrow.
It's important to realize that proof-of-work and de-centrality to establish trust, are just a means not an end.

Ends
~~~~

* Digitized (and standardized!!) assets
* A trusted ledger that provides transparency (e.g. if trusted parties are corrupt, society can witness)
* Efficient system, no expensive middlemen that can be replaced with technology

Characteristics of real assets
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Unlike bitcoin or gold, there are many assets that are linked to a central party. For stock its the company behind it and for real estate it's the local authority that allows you to claim the land.
So the following is actually a valid question: Do you need a global de-central ledger to record asset ownership claims that can be overruled by authorities?

Private blockchains
-------------------

Private blockchains do not provide the de-centrality public blockchains provide. Which was Bitcoin protocol's core innovation.
Maybe, for many assets, private blockchains could be a good enough *means* to the above *ends*.

Current private blockchain implementations often have a specific, narrow, focus.
They are tied to a specific group of companies that work together. It brings transparency, efficiency and middle men can be cut out.
However it forces, often non-tech companies, to maintain a ledger themselves.

Example: bookstore vouchers
~~~~~~~~~~~~~~~~~~~~~~~~~~~
Book vouchers can usually be redeemed at many different bookstores.
Blockchain technology could be an efficient solution to register transactions.
But does it make sense to ask non-technical companies such as bookstores to each maintain a peer of the private network?

Temporary sweet spot
--------------------
With so many unanswered questions and the ambition to go live today and not in 2018; we are currently experimenting to see if a **general purpose** private blockchain fits real, regulated, assets best.

.. note:: Maturing of technology might gravitate the sweet spot towards more de-centrality (public blockchains) in the future.

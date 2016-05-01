.. _commercializationplan:

Commercialization Plan
======================

This section describes some options for commercialization and
technology transfer that are being considered for DIMS deliverable
products.

.. _intellectualProperty:

Under the terms of the Contract, Section C.3.4, the products of this project
are to be released as open source under a selected open source license. As
described in Section :ref:`approvedLicense`, this license is the
Berkeley Three-Part license.

.. _technologytransfer:

Technology Transfer
-------------------

No intellectual property disclosures to the University of Washington will
result from this project. All technology tranfer will result from uniform
access to the public of the released open source code and documentation.

.. _csirtgadgets:

CSIRT Gadgets Foundation
~~~~~~~~~~~~~~~~~~~~~~~~

Conversations with Wes Young and Gabe Iovino of the `CSIRT Gadgets Foundation`_
indicate that their foundation may be a good place for forks of the DIMS code,
configruation, and documentation repositories to be housed and maintained
similarly to the way the `Collective Intelligence Framework`_ is maintained.
Additionally, there are opportunities working with the foundation to
enhance CIF using DIMS products and lessons learned.
This would be a natural place to take the techniques in system administration
automation, Docker containerization and CoreOS clustering, and continuous
integration of source components and system configuration.

.. _CSIRT Gadgets Foundation: https://csirtgadgets.org/
.. _Collective Intelligence Framework: http://code.google.com/p/collective-intelligence-framework/


.. _farsightsecurity:

Farsight Security
~~~~~~~~~~~~~~~~~

Farsight Security has expressed an interest in supporting continued development
of DIMS components with letters of support and other political and social acts,
but desires to be a client in future collaborations rather than a volunteer
contributor. They have been very generous in making architectural changes that
help integrate DIMS components with the new (and soon-to-be publicly released
**Trident** portal system) and appreciate feedback from red teaming done in
conjunction with this project.

Dr. Paul Vixie recently published a blog post, `Magical Thinking in Internet
Security`_ in which he points out the problem of complexity in implementing
security solutions, especially one's designed to detect and respond to
computer intrusions (while not being the *source* of intrusions, due to
security weaknesses in these complex systems that are not addressed
by the limited resources often invested in implementing these systems.
He starts his conclusion with this statement: "Increased complexity without
corresponding increases in understanding would be a net loss to a buyer."
DIMS products are intended to help shift the equation put forward
by Vixie, by helping make a less complex, more transparent, and easier
to secure platform than may otherwise be produced by trying to
leverage open source security tools from scratch.

.. _Magical Thinking in Internet Security: https://www.farsightsecurity.com/Blog/20160428-vixie-magicalthinking/

Further conversations with Farsight will explore possible interest in grants or
contracts to provide financial support for any further system integration
efforts.


.. _ci:

Critical Informatics and PISCES Northwest
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

The Critical Informatics (CI) business model is complementary to the feature
set of DIMS. The PI and the principal co-founder of CI (Mike Hamilton) have
worked together on the concepts for regional collaborative incident response
under various forms of DHS funding going back to 2008.

Critical Informatics will be supporting the newly-formed not-for-profit
entity known as the Public Infrastructure Security Collaboration
and Exchange System (PISCES-NW, for "North West").

The PI will be engaged for a limited period of time in the initial
phase of the PISCES-NW contract project, focused on assisting
with implemention of selected DIMS open source products as
requested by PISCES-NW.

.. _cri:

Cyber Resilience Institute
~~~~~~~~~~~~~~~~~~~~~~~~~~

The PI was invited to be on the Board of Directors of the Colorado-based
Cyber Resilience Institute (CRI). DIMS products will be demonstrated to
the CRI Board and considered for inclusion in pilot projects that
CRI is pursuing, possibly in collaboration with educational institutions
in the state of Colorado.

.. _other:

Other Security Companies
~~~~~~~~~~~~~~~~~~~~~~~~

Conversations have taken place with other "stealth-mode" computer security
companies, both in Washington state and other states. Because of non-disclosure
agreements, they will not be directly named here. The discussions have involved
the possibility of using and contributing back to the DIMS open source code
products, using them to complement internally-developed commercial products
and services, and/or implementing custom deployments of DIMS+Trident
components for customers to use in forming and operating trusted information
sharing and security operations. Possible partnership between several of
these companies is on the table, which could greatly accelerate continued
development of capabilities produced under the DIMS contract.

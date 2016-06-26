.. _introduction:

Introduction
============

The Verizon Data Breach Investigation Report [DBIR16]_, one of the most
highly-cited sources of information on data breach causes, reports that almost
40% of intrusions are targeted at servers (p. 9), 63% of breaches are due to
weak, default, or stolen password (p. 20), and about 1/3 of all breaches are
due to mistakes and misconfiguration, privilege misuse, and other factors
related to computing *infrastructure* apart from vulnerabilities in software
(p. 22).  In December 2015, Forbes estimated that the market for cybersecurity
products and services in 2015 was \$70 Billion and would reach\$170 Billion by
the year 2020. [Mor15]_

Open source software makes up the foundation of the Internet as we know it
today. OpenSSH, OpenSSL, NTP, and GnuPG are examples of successful open source
software used in many products, both open source and commercial.
Vulnerabilities like Heartbleed (CVE-2014-0160) have served as a wake-up call
for the need to improve the development and maintenance processes of these open
source projects to create a more secure foundation.  The `Linux Foundation Core
Infrastructure Initiative`_ aims to "speed the pace of open-source innovation
while dramatically reducing global threats to online security." They do this
with the `Badge Program`_ using detailed `badging criteria`_ establishing
an "open source secure development maturity model."

But what about the operating systems, libraries, and configuration of services
that make up the *infrastructure* within which the Badge model is supposed to
be followed? That hidden layer of infrastructure must also be built securely,
expand securely, and be maintained securely, otherwise the source code for
those open source products and the security operations functions are put at
risk.  The CII `Badge Program`_ points to the `GitHub Security`_ policy and
`Heroku Security`_ policy, both of which are great high-level lists of
*what to do* (but not *how to do it* using any specific Linux distribution that
a group would use to build a distributed system). What if a group can't or
doesn't want to use GitHub and Heroku, or wants to operate within a
*private cloud* deployment?

Not-for-profit or volunteer organizations who produce open source
software, or those providing affordable managed security services to local
government based on open source tools, must pay attention to the findings of
the DBIR and address the infrastructure security requirements, while doing
so on very limited budgets.

Those tasked with setting up and administering their own infrastructure,
integrating multiple open source tools in a scalable or distributed deployment
are not only faced with figuring out how to do it securely, but must also deal
with the choices made by other teams who produced the open source tools to be
integrated (which often are mutually exclusive in terms of base operating
system distribution, OS release version, prerequisite libraries, and
programming languages used by the services to be integrated.)

To sum up, we can paraphrase an old joke attributed to Jamie Zawinski (`Source
of the famous "Now you have two problems" quote`_):

.. pull-quote::

    *Some people, when confronted with the problems just described, think
    "I know, I'll use open source security tools!"  Now they have two problems.*

..

The remainder of this document will discuss :ref:`valueproposition`, :ref:`licensingplan`,
and :ref:`commercializationplan`.

.. References and footnotes follow.

.. _Linux Foundation Core Infrastructure Initiative: https://www.coreinfrastructure.org/
.. _Badge Program: https://www.coreinfrastructure.org/programs/badge-program
.. _badging criteria: https://github.com/linuxfoundation/cii-best-practices-badge
.. _GitHub security: https://help.github.com/articles/github-security/
.. _Heroku security: https://www.heroku.com/policy/security
.. _Source of the famous "Now you have two problems" quote: http://regex.info/blog/2006-09-15/247

.. [DBIR16] Verizon. 2016 Data Breach Investigations Report. http://www.verizonenterprise.com/verizon-insights-lab/dbir/2016/, April 2016.
.. [Mor15] Steve Morgan. Cybersecurity Market Reaches $75 Billion In 2015; Expected To Reach $170 Billion By 2020. http://onforb.es/1QDaK3D, December 2015.

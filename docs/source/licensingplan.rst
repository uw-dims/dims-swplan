.. _licensingplan:

Licensing Plan
==============

This section represents guidance obtained from an initial conversation
in the Base Year with Peggy Hartman, and multiple conversations with
Fred Holt in 2015 and 2016.

Compatibility of Open Source Licenses
-------------------------------------

Wikipedia has a good description of what constitutes a
`Permissive free software licence`_, which is a concern when integrating
open source projects.  Figure :ref:`licensecompatibility` from this page
is included here (under the terms of Creative Commons “Attribution-Share
Alike 3.0 License”).

.. _licensecompatibility:

.. figure:: images/Floss-license-slide-image.png
   :alt: License compatibility between common FOSS software licenses according to David A. Wheeler (2007)
   :width: 70%
   :align: center

   License compatibility between common FOSS software licenses according to David A. Wheeler (2007)

..

.. _Permissive free software licence: https://en.wikipedia.org/wiki/Permissive_free_software_licence

.. _approvedLicense:

University approved release license
-----------------------------------

Initial guidance from Peggy Hartman indicated that University of Washington
preferred that software produced by the DIMS team be released under
the Berkeley Three-Part license (also known as *BSD-3*).

.. include:: license.txt
   :literal:

This is a simple license that falls into the *permissive* category of open
source licenses.
.. todo::

    Add graphic Fred sent me about comparison of licenses.

..

Considerations for release of DIMS project source code
------------------------------------------------------

.. attention::

    This subsection incudes information obtained in conversations with Fred
    Holt, who has worked on intellectual property and technology transfer
    issues with the University of Washington Office of Technology Transfer.
    
..


The GPL has over 20 years of history of controversy for its terms and
conditions.  Some of this controversy resulted in a slightly less restrictive
and narrower license known as the Lesser GPL (LGPL).

Part of the controversy over the GPL surrounds the time in which it came to
exist and the style of programming languages at the time that were heavily
slanted towards *compilation* and *linkage* (that is, writing *source code*,
running a *compiler* on the source code to produce *object files* and *object
libraries*, running a linker on the *object files and libraries* to produce an
*executable binary image* (also commonly called an *executable* or *EXE* file).
The GPL was targeted at these compiled executables, so if you used a
``Makefile`` to compile and link source code with libraries released under the
GPL, then under the spirit of the GPL's terms, your program and its modules
also had to be released under the GPL.

In today's programming environment, things are much more complicated. Languages
like Python act more like interpreters than compilers, though they do produce a
post-parsing form of binary code that helps speed execution by reducing
redundant parsing. Modules are imported into Python programs (often by loading
them into the directory hierarchy in which the Python interpreter stores its
own module source files).  Languages like Java similarly produce a *bytecode*
intermediary binary format file that is executed by a bytecode interpreter
known as the Java Virtual Machine (JVM), rather than being linked into a
stand-alone executable, with modules used by the program.

This is complicated even further by following the Unix philosophy of programs
being simple and doing one thing very well, and those program being used with
pipelining and other execution invocation mechanisms to compose these simple
functions into higher-level more complex functionality, which can then be
further combined, and on and on. This raises questions like, "`Is a program
that forks a GPL-licensed program via a system or vice versa call derivative
work?`_" and -- specifically to the DIMS project, which uses Ansible -- "[Does]
the GPL license imply that my [Ansible] plugins are also GPL?" (see `Ansible
issue #8864`_)

Given the spirit of intent of the GPL, the following guidance will be applied
to DIMS code:

.. > So — [[ and these examples do not have clear boundaries ]] - 

* If source code is compiled and a GPL licensed module linked into it,
  then the resulting executable should be released under the GPL.

  .. note::

     The exception is the case where the GPL code may just facilitate
     one “layer” of a complex program, where the LGPL is more applicable.

  ..

* If we invoke a GPL program in a shell (even with arguments) then the other
  levels of the larger program, above and below the shell that invokes the
  GPL program, can be released under a different license (e.g. BSD-3)

  .. note::

    Look for a good boundary around any GPL code, which respects the
    spirit of the GPL.

  ..


* `Ansible issue #8864`_

.. _Is a program that forks a GPL-licensed program via a system or vice versa call derivative work?: http://www.ifross.org/en/program-forks-gpl-licensed-program-system-or-vice-versa-call-derivative-work
.. _Ansible issue #8864: https://github.com/ansible/ansible/issues/8864


.. title: Free Software and Computer Security
.. slug: free-software-and-computer-security
.. date: 2015-06-22 21:32:59 UTC
.. tags: linux, python, free software, information security, computer
   security, draft
.. category: 
.. link: 
.. description: Security advantages and potential pitfalls with Free Software
.. type: text

I have been thinking much about information security over the last few
months.

Over the years I have thought about the relative merits of `free
software` versus non-free.

Free as in freedom, or logicel libre if you prefer.  Free software
comes with important freedoms.  You are free to examine how it works,
make changes and experiment.

Free software is everywhere, for example, `openssl`_ is used in many
different operating systems.

Your security depends on free software
======================================

Even when you are using non-free, you are almost surely using lots of
free software at the same time.  Depending on how that software is
licensed you might be able to find just which software is used.

I find one key differentiation in licenses is in the restrictions they
choose to put on the licensees.

So the most permissive licenses tend to be along the lines of, "here
is some software, do what you like with it, don't sue me".

Other common clauses
--------------------

Others might insist on attribution (for example if you modify it and
pass the resulting application onto somebody else) and have things to
say about trademarks etc.

You can find broader discussion of licenses at the following links:

* find some good license discussions
* more..

GPL v non-GPL
=============

The key clause of the `General Public License`_ is that it insists
that if you pass on the same rights you received to any that you
pass it onto.

The idea is that recipients should have all they need to explore,
modify and experiment with the code.

Affect of the GPL
=================

Things are complicated.  On many levels the major effects apply
regardless of the license.

The non-GPL have been adopted more readily by proprietary vendors, for
example `Apple's OS is derived from BSD Unix`_.

Python has a BSD style license.  Python seems to like to make it avaiable to
anyone who is interested in the language.   It does say that if you
create a derivative work, that you need to include a brief summary of
the changes made to python.

The license begins with some history of python, and some background on
`Guido van Rossum`_,

** CHECK THIS **

The GPL has also been used as a way to encourage to license the
product under a more permissive license.  One notable example was
`MySQL`_ which was licensed uder the GPL but that enabled the company
doing the bulk of the deveolopment and driving the project to get
license income from those that appreciated the support.

It allowed other businesses to build a business on top of MySQL, but
with their own custom adaptions.  Often these adaptions would
eventually end up in the project itself.  At some point it is better
to share the maintenance burden of a new feature.  Often that point is
now.

Python makes itself accessible and hence it has become ubiquitous.

The main effect of licenses is that the non-GPL software tends to be
more widely adopted by commercial organisations.  The main reason is
it allows them to produce derived works and not have to distribute
their own customisations and improvements.

However, for smaller commercial organisations it is generally more
effective to work with the project itself and share their work.

Keeping your fixes proprietary comes with costs as well as benefits.
A number of questions you need to ask are:

* Does this enhancement give me a significant competitive advantage?
  
* Why has nobody else done this already?
  
* Are people achieving the same result through some other feature or
  product I do not know about?
  
* How long will it be before the project implements a feature like the
  one we have build?
  
* Would we be better off sharing our feature and hence having more
  control over the future development?

Benefits of free software
=========================

provided tools others can use freely.

supports free experimentation, gives a world of ideas which you can
explore with others

created tools to help with collaborative working

found ways to collaborate across the internet

enabled local people to gain skills needed in their environment

runs on old hardware

it is a significant voice in the debate on information security and
privacy.  It will very likely play an important role.


Security benefits
=================

Free software
-------------

Since people have access to the software and are free to experiment
and explore how it works they can look for potential security holes,
report the problems and perhaps fix them if they have the skills.

Of course, the bad guys also have this advantage over non-free
software.



Sharing your work openly
++++++++++++++++++++++++

When you work with free software you are showing the world your code.
This takes a certain amount of courage.  Anyone who has taken part in
a code review knows that showing your code to others is baring your
soul.

Most effective code shops have some form of code review in their
development process.  Two pairs of eyes are always good.  It helps
share knowledge, educate both parties and create better software.

Once developers get comfortable with sharing with their peers, sharing
with the wider world becomes less daunting.

Positive feedback can be very helpful here: you get an immediate
benefit for sharing.

Many software engineers (and I include myself in this) are quite
insecure about their code.  Most programmers are `sort of average`_,
but knowledgeable enough to know that with more time and research
their code could be better.

Regardless, code that is shared openly is likely going to be of a
`higher quality`_ by depending on the metric you choose to use to
measure quality.  The authors of the code will likely care about their
reputation in the free software community and hence take care to share
quality work, or at least identify the code as a quick hack or
whatever.

Potential sources of vulnerabilities in free software
-----------------------------------------------------

Simple bugs
+++++++++++

Malicious contributions
+++++++++++++++++++++++

Compromise of repository
++++++++++++++++++++++++


Non-free software
-----------------

With non-free software you are working with a black box.  You get to
choose inputs and observe outputs.  If you are lucky you can learn
about how the code works, but it is much harder than 

Reverse engineering
+++++++++++++++++++

If you have an executable there are tools that will allow you to take
the binary code and create human readable assembly code.  This is
generally missing comments and variable names.  It is a low level
description of the code, closer to the final op codes that a computer
runs.

However, for those with skill and experience, reverse engineering is a
powerful technique.

Sometimes the license will explicitly say you must not reverse
engineer the code.  Of course, bad guys will not necessarily obey the
license.

However, security researchers will often decide not to break the
license.  The result is that only the bad guys are looking closely at
the code for vulnerabilities.

This is not a place you want to be.


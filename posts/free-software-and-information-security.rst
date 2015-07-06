.. title: Free Software and Information Security
.. slug: free-software-and-information-security
.. date: 2015-07-03 23:29:17 UTC
.. tags: meta data, python, GPL, information security, free software,
   Snowden, draft
.. link: 
.. description: Not sure yet
.. type: text

I have been thinking a lot about the relative merits of free and
non-free software and have started writing a piece about that.

This week a the Intercept published a piece on how the NSA's *google
on steroids*, `XKEYSCORE`_ works under the hood.

`Micah Lee`_, an expert in information security, and Linux enthusiast
was heavily involved in the piece.  It is always good when people who
really understand the technology are involved like this.

XKEYSCORE is built with the free software, LAMP stack: Linux, Apache,
MySQL and Perl/Python/PHP.  RedHat are providing the Linux.

So, the NSA uses free software for its critical infrastructure.
Further, it depends on free software to keep its operations secure.

This revelation fundamentally changes the debate about the relative
merits of free and non-free software from a security point of view.

On the one hand it is a ringing endorsement for LAMP:  it is secure
enough and robust enough for critical infrastructure.

Writing about information security is difficult.  Every facet is
double edged, sometimes multi-edged.

Clearly the NSA engineers understand Linux very well.  They are using
it to develop their systems.  They know how to be productive in that
environment.  In short, free software works.

They themselves work in a very collaborative environment.  They have
highly intelligent, passionate and ingenious people who love a
challenge.  And they use free software.

They will understand how Linux works at a pretty deep level and know
how to make it run well, how to get the most out of it.

So do Google and a multitude of other organisations doing high
performance computing, where shaving 5% off the resources can make a
big impact.  Mostly though they will be looking to cut things by an
order of magnitude, or two.

We are seeing daily how insecure data that is stored on computers is.
Then there is the integrity of that data?  How much of it can we
really trust?

Three types of information
==========================

Individuals have three types of information based on how many people
they wish to share that information with:

* information they do not wish to share with anyone else

* information they are happy to share with anyone and everyone

* information they wish to share, but only with a strict subset    
    
The first two are just about feasible to handle with today's
technology and software.

The third is extremely difficult with today's technology.  Witness all
the security breaches in the news.

It may not even be a technological problem.  Rather, it is a social
issue.  Or rather it is an immensely complex mix of social issues.

In the context of information on computers there are so many issues it
is hard to know where to begin.  It looks like a fairly radical
re-think is in order.

The good news is there is a lot of excellent work being done in the
free software community.  There are many very smart people working on
some very difficult problems and making good progress.

Meanwhile there are others that are fixing problems in existing
systems and helping the users of their software to plug holes too.
This is how free software works.

Now in the public debate we are often given stark choices.  *If X
happens the sky will fall in.*

These arguments reinforce the mistaken belief that the choices are so
stark or indeed so simple.

As an example, there is a thing called *homeomorphic encryption*.  The
idea is to take some data and to turn it into something else that has
the same sort of structure, but has thrown away some information in
the process.

There is a whole cottage industry of people these day who will sell
you tools to *anonymise* data, mostly for privacy reasons.

The data is invaluable for strategic planning, but it is very
difficult to get the balance between respecting privacy and the good
of the community.  And anonymising data is really, really hard to do
well.

Especially if others are anonymising related data.  And they are.

I explain homeomorphic in more detail later.

Everyday Living on a small island
=================================

I live in Bermuda.  The island is small.  There are about 1.5 degrees
of separation, everybody knows everybody.

Children learn from a young age how fast the Bermuda grapevine can
be.  If they are doing something they shouldn't be doing the news
invariably gets home to mum before they do.

As a result, Bermudians tend to be very respectful of people's
privacy.  They have their own forms of *homeomorphic encryption* in
the way they relate stories, often using terms such as *ace-boy* or
*ace-girl* to protect identities.

Security researchers can learn a lot from the way these people handle
information.


Cuban Ubuntu
============

Yet another interesting twist in the world is the restoring of more
normal relations between Cuba and the US.

I learned the other day that the Cubans have their own version of
Ubuntu, callend `Nova`_.

Who are you going to trust?
===========================

Information security currently comes down to *who or what are you
going to trust?*.

For now, I am placing my trust in the free software community.  It may
not be perfect, but by my judgement it is by far and away the best
option right now.

Homeomorphism
=============

There is a thing in mathematics called `homeomorphism`_.  I expect the
term turns up in many other areas too.

In mathematics it means some sort of trasnformation of an object that
leaves certain properties unchanged.   There are different kinds of
homeomorphism of different branches of mathematics.

In topology, if the objects are made of rubber that can be deformed
and you can change your object into the other one without doing things
like cutting the rubber or filling in holes, then you have created a
homeomorphism.

Topologists are people who think a mug and a doughnut are the same
thing.

Shannon
=======

For those interested in some mathematics behind information,
`Shannon's Theorem`_ is a good place to start.


.. _XKEYSCORE: https://firstlook.org/theintercept/2015/07/02/look-under-hood-xkeyscore/

.. _Micah Lee: https://firstlook.org/theintercept/staff/micah-lee/

.. _Nova: https://en.wikipedia.org/wiki/Nova_(operating_system)

.. _Shannon's Theorem: https://en.wikipedia.org/wiki/Noisy-channel_coding_theorem

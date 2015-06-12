.. title: Cyber espionage nightmare and the case for open data
.. slug: cyber-espionage-nightmare-and-the-case-for-open-data
.. date: 2015-06-12 18:18:23 UTC
.. tags: cyber risk, information security, open data
.. category: 
.. link: 
.. description: 
.. type: text

I keep starting posts on information security and the dismal state of
computer security and then another day arrives with another story of
data breaches and the post no longer seems relevant.

Today started with news of a big `SNAFU by a Malaysian telco`_.  `Part
2`_ of this excellent `history of internet security`_ explains how
this giant hole in the internet has been there for a long time and
been the cause of some spectacular breakages in the past.

As the article explains, it is really a consequence of the design
philosophy of the internet.  The aim was to create a robust network
that could self-heal.  The focus was on creating a system that would
allow communication after a catastrophic event such as a nuclear war.

The `Border Gateway Protocol`_ controls routing of packets through the
internet.  If a router says it offers the best route to a particular
host, the BGP is OK with that.  BGP started life as some scribblings
on three napkins over lunch.  Now it is fundamental to the working of
the entire internet.

Now, if you think about the scenario for which it was designed, back
in the 1980's this is not such a bad feature: a nuclear war has
destroyed lots of infrastructure, so if a node in the internet says,
"Hey, I can help you out", why wouldn't you give it a go?

The problem is that most of the internet traffic is unencrypted, so if
a malicious party pretends it is the best route to *google.com* it
gets all the traffic, in clear.  Not so good.  And it stops packets
from going where they are intended at the same time.  

The first part of the history of internet security explains how
the design in effect delegated responsibility to the end points on the
internet.  In short, every person connected to the internet is
responsible for keeping it secure.   Now this worked pretty well in
the days when you needed an expensive computer to connect and the
people running that computer were probably also doing some of the
coding that keeps everything running.

But now the whole world is online, the trust model is somewhat broken.
In fact, it is remarkable how well the whole thing does work.  We
should not lose sight of this: the system works pretty well at times.
In fact, it works wonderously well for data that you do not mind
sharing with everyone.  If you have secrets, then it starts to get
more problematic.

We hear stories such as this `cyber espionage nightmare`_.  Let's
assume the account is accurate; it should be noted that this whole
area of computer security is full of smoke, mirrors and snake oil
salespeople, which further complicates assessing the real risk out
there.

At this point, it is quite clear that most corporations and even
`governments`_ are fundamentally incapable of protecting data.

Further, much sensitive data has already leaked out.  Many
organisations are unaware how much data has been leaked.  The OPM
apparently discovered their breach when a marketing team was giving a
demo of their intrusion detection software.

Like the cold war that gave rise to the internet itself, there is an
arms race going on.  Unlike the cold war, though, once you have lost
your secrets they are gone for good.

Now in the short term, the situation is not good.  Many people's
secrets will be leaking out to a wider audience.  

Much of the damage is mitigated by the fact that most internet users
are not malicious.  For example, when Sony had its email archive
leaked and posted online, most people, conscious of how they would
feel about others trawling through their inboxes left it well alone.

But if the party that acquires the secrets has malicious intent, then
damage will ge done.  The `cyber espionage nightmare`_ article talks
about economic espionage and the stealing of corporate secrets.

Holes in the internet will undoubtedly be plugged.  Widespread use of
encryption would seem to be desirable.  However, at some point people
need to read the actual data, it will be decrypted and so you have to
ensure that only happens on secure systems.

Such things are pretty hard to come by.  Securing computers against
the most determined attackers is extremely difficult with today's
tools.

If your secrets are not too valuable to others then you may be OK.
Further, if you are a bit more secure than other equally interesting
targets you may be OK.

One solution that will always work is not to store secrets on your
computers.   How much of your data is really secret?   Might you be
better off sharing your precious intellectual property with everyone?

It turns out large numbers of people are doing just that.  With free,
open source software, open data and open scientific research.  Rather
than burdening yourself with having to keep all this information
secret, work in the open.  Collaborate with others, together build a
better mousetrap, a better society for everyone.

The renaissance was very much driven by the sharing of knowledge
generated by the invention of the printing press.  The internet takes
this to a whole new level.  Humanity is sharing ideas like never
before.  New inventions come when people put together ideas from
different fields.

The challenge today is not keeping your own ideas secret, rather it is
keeping pace with new developments driven by the open sharing on the
internet.

The internet was designed for sharing information.  If you are using
to share secrets, it probably won't work out so well for you.

The company in the `cyber espionage nightmare`_ may well have been
better off sharing its knowledge and focussing at being the best in
its field, benefitting from contributions from others and from not
having to waste valuable resources protecting secrets it cannot hope
to keep.

If you cannot compete with others who have to ship their products half
way round the world to beat you then maybe you are not good enough at
your business.

.. _history of internet security:   http://www.washingtonpost.com/sf/business/2015/05/30/net-of-insecurity-part-1/
   
.. _cyber espionage nightmare: http://www.technologyreview.com/featuredstory/538201/cyber-espionage-nightmare/

.. _Part 2: http://www.washingtonpost.com/sf/business/2015/05/31/net-of-insecurity-part-2/


.. _Massive BGP leak: https://www.bgpmon.net/massive-route-leak-cause-internet-slowdown/

.. _Border Gateway Protocol: https://en.wikipedia.org/wiki/Border_Gateway_Protocol

.. _OPM breach: http://www.wired.com/2015/06/opm-breach-security-privacy-debacle/

.. _governments: `OPM breach`_

.. _SNAFU by a Malaysian telco: `Massive BGP leak`_

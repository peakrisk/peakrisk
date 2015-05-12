.. title: Unreliable internet service providers are part of the security problem
.. slug: unreliable-internet-service-providers-are-part-of-the-security-problem
.. date: 2015-05-07 16:33:35 UTC
.. tags: cyber risk, computer security, draft
.. category: 
.. link: 
.. description: Why unreliable internet is a security risk
.. type: text

Today my internet connection has been pretty much broken.

Many sites are just not responding, including bbc.co.uk.

Some larger sites, such as google and facebook are responding.  As is
the ever dependable linux.ie.  Sites hosted here in Bermuda are mostly
working well.  Another reason why local hosting is important.

Using the linux utility `mtr` it seems stuff is getting routed
successfully out of Bermuda, then hitting a black hole.

I called the ISP and was told *the internet is down*.  There is no
information on the ISP's website about there being an outage.  When
you call the support line, you get a message about their new products
*for educational purposes*.   Er, no, that is for marketing purposes
not educational.  If you want to educate then perhaps have a message
about the on-going problems instead.

Why is flakey internet a problem?
---------------------------------

The internet here in Bermuda is at best unreliable.  Now, accepted we
are a small island in the middle of the ocean and that presents some
challenges.

The problem is that internet users here get used to the internet being
unreliable.  So when it doesn't work like it should it is easy to
dismiss it as *the fine ISP is having one of its SNAFU's*.  

Further, when systems are not working, system admins end up tinkering
with settings to try and fix and diagnose the problem: maybe it is a
problem on my end not the ISP?

And this inevitably leads to lowering of security while the
troubleshooting is done.

And what if there isn't really a problem with my ISP but instead my
own system is under attack?

So, if you are an unreliable ISP, who fails to give clear information
to your customers when there are problems you are really saying, "We
do not care about your security".

System admins
-------------

The job of a system administrator is not an easy one.  They have to
keep things secure (an impossible task), whilst keeping things running
so people can do their jobs.  

This `IT confessions`_ thread on Reddit gives an idea of the world in
which they are working.  Often only 1-2 people to look after an office
of 80 or more.  

Many admins will lock down machines and impose (industry standard)
rules.  However, these can be counter-productive: if users can't get
their work done they will find ways round the rules, often resulting
in a worse situation than not having the rules in the first place.

It is not uncommon for admins to see their users as the problem.  In
many cases these users are not computer experts (nor should they be),
but this leads to frustration when they make demands of the system
admin. 

The real problem is that securing computers is a close to impossible
task, if you also want your users to be able to continue to do their
jobs. 

.. _IT confessions: http://www.reddit.com/r/sysadmin/comments/35am51/it_sins_confession_booth/

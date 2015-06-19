.. title: Teaching with pi's
.. slug: teaching-with-pis
.. date: 2015-06-19 18:14:24 UTC
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text

This week I spent two half days trying to teach about free software
with raspberry pi's.

The students were all local, in full time further education in IT
fields and hoping to have a career in IT.

There were 4 students, a mixed group.  Fortunately for me, a previous
graduate of this summer programme came along to help out.

Day 1
=====

The first session was a lesson in the problems of working with tech in
education.  I had made a visit to the room for the training the
previous week.

I was supplying raspberry pi's and SD cards, but we needed monitors,
keyboards, mice, HDMI cables and wired network connections.

Now we were only able to find monitors with DVI ports, not HDMI and
only two monitors.  Fortunately, I had DVI to HDMI adaptors and we
managed to cobble together the remaining bits and pieces.

I'll skip the problems we had connecting to the network and perhaps
cover that in a future post on security and other matters.

Free software was mostly new to the students.  Where to begin.  I
wanted to show them linux, but through the command line.  I wanted
them to start to develop a better understanding of how a computer
actually works, one of the goals the raspberry pi project shares.

My helper was fantastic.  Since there were two pi workstations set up,
he worked with one pair of students and me with the other.

One goal on the first day was to introduce the students to version
control using `git`_ on the command line.

Now we soon hit the editor problem.  There is always the dilemma
between showing powerful tools with a steep learning curve and simple,
quick to learn tools in this sort of training.

I wanted to give the students a glimpse of `emacs`_, in part because
it is a classic free software tool.

I first encountered emacs around 1985 when attending an `Introduction
to Unix`_ course at a local technology college in the UK.  The course
was a couple of days and they taught us some simple C-shell and an
introduction to Unix systems.

Since an editor was needed for the examples, they showed us `emacs`_.
I recall writing a review to the effect that whilst emacs seemed to be
super powerful, it took a disproportionate amount of the time for the
course.

My next experience with emacs was around 1989.  My workplace had
acquired shiny new Sun workstations.  Running Unix.  So the first
thing I needed was an editor.  A colleague explained there were two
practical choices: emacs and vi.  Emacs had a vi mode, so basically
that sealed it.  Emacs it was.

This time I was going to be using it to write code.  An investment of
a few hours learning how to use it well seemed worthwhile, so I read
the tutorial.  Soon I was hooked.  This thing was so much more
powerful than anything I had used before.

I am still using emacs, some 25 years later.  I've used it to edit
code in fortran, C, perl, tcl, python, lisp and who knows what else.
I've played tetris, read email, browsed newsgroups, read twitter, run
ipython notebooks, used git, read man pages and who knows what else.

For the training though, I probably should have just pointed the
students at this raspberry pi page on `editors`_.

By the end of the first session the students had created a git
repository and were able to make changes to files, state the changes
and commit them to the repository.

Day 2
=====

I had a bit of a re-think after the first session.  We decided to
bring in some more equiment to give us more options in the room.

The students are on a 3 month programme, involving internships in
local firms, with 1 week per month in training.

They also have to do some sort of project for the course.  One idea
they are considering is to create a website which provides information
on the public transport on the island.

I decided to structure the afternoon around how they might go about
this if they wanted to run it as a free software project.

This gave an opportunity to introduce the students to `github`_ and
build on the introduction to git that we had started in the previous
session.

The bus application is challenging here in Bermuda as much of the data
needed for the application does not appear to be available in machine
readable form.

For most free software bus applications having your schedule and route
data in the `General Transit Feed Specification`_ allows you to take
advantage of a lot of work done in other jurisdictions.

The good news for Bermuda is that its bus and ferry network is small,
so even if this data has to be entered by hand it should not take too
long.  Further, the students could always concentrate on one or two
key routes while the iron out the glitches.

I had hoped to introduce a little python programming, but this will
have to come in later sessions.

In the meanwhile, this `advanced git`_ talk from this year's PyCon may
be helpful to get a better understanding of how git actually works and
introduce some more advanced concepts.

The PyCon videos are all in the *PyCon 2015* channel on youtube.  I
also recommend Jacob Kaplan-Moss's `keynote`_ to anyone unsure about
whether they have the skills to be a programmer.

I am looking forward to being involved with these students over the
summer.  Hopefully, they are about to start doing some great things
with free software.

.. _General Transit Feed Specification: https://developers.google.com/transit/gtfs/reference

.. _git: https://git-scm.com/
	     
.. _Jacob_Kaplan_Moss: https://www.youtube.com/watch?v=hIJdFxYlEKE

.. _keynote: Jacob_Kaplan_Moss_

.. _Advanced Git: https://www.youtube.com/watch?v=4EOZvow1mk4    

.. _Editors: https://www.raspberrypi.org/documentation/linux/usage/text-editors.md

.. _emacs: http://www.gnu.org/software/emacs/

.. _github: https://github.com

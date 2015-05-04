.. title: Data, data, everywhere, nor any drop to drink
.. slug: data-data-everywhere-nor-any-drop-to-drink
.. date: 2015-04-30 17:01:06 UTC
.. tags: 
.. category: 
.. link: 
.. description: opendata
.. type: text



.. figure:: http://upload.wikimedia.org/wikipedia/commons/8/80/Gustave_Dore_Ancient_Mariner_Illustration.jpg
   :align: right

   Gustave Dore Ancient Mariner Illustration, licensed under Public Domain via `Wikimedia Commons`_.


Satellite data
--------------

I started looking at this data after being inspired by Chris Waigl's
PyCon talk on `Satellite mapping for everyone`_.  Chris gave an
introduction to some of the python tools you can use to look at this
data.

She mentioned some websites where you can find data from various
satellite missions and showed how to work with the data and just what
sort of data is available.

There really is a wonderful array of data available.  The process of
exploring all this can be time consuming, but fun.  There is a lot of
fascinating work being done.

I was hoping to find images in and around the time of the hurricanes.
With high enough resolution I believe it should be possible to use
image processing software to help with damage surveys.  For example,
it should be possible to spot blue tarpaulins placed over damaged
roofs, or indeed the roof damage itself.

I picked Landsat, pretty much based on Chris's talk.  I found two days
either side of the hurricanes in Bermuda last October for which there
were images available for.

So far so good.  But to get the higher resolution data you had to
register and obtain a key to gain access to the downloads.  These are
large, around 1GB per image, so it is reasonable for whichever agency
is supplying the images to know a little about those downloading the
data. In particular, be able to contact them if putting an
unreasonable load on their servers.

Now for Bermuda we only really need about 1% of the data which covers
the few square miles around the island.   This is much more
manageable, so it feels it would be good to be able to host the data
locally.  This is something I expect I will return to.  

There is still much to do here.  Chris noted that *you will learn
coordinate systems*.   Up to now I have managed to avoid this, just
slicing the `numpy`_ arrays that `rasterio`_ gives me as I read the
images. 

I need to learn how to pull out a window from one of these images by
specifying the lat/lon box defining the area to extract.  Better
still, I could do with a number of pre-defined boxes that pull out
interesting areas of Bermuda, for example each Parish.

Satellite data for smaller jurisdictions
----------------------------------------

Most satellite data is collected by expensive national and
international space missions.  Many of the missions are aimed at
creating a global resource, but generally focussed on the nations that
funded the missions.

`Global Precipitation Measurement`_ mission has a number of data sets
available.  These are typically at the 0.1 degree resolution, which
corresponds to 7 miles on the ground.  The temporal resolution is
good, a new image is available at 30 minute intervals.  Further, the
project aims to::

    intercalibrate, merge, and interpolate "all" satellite microwave
    precipitation estimates, together with microwave-calibrated infrared
    (IR) satellite estimates, precipitation gauge analyses, and
    potentially other precipitation estimators at fine time and space
    scales for the TRMM and GPM eras over the entire globe.

For Bermuda, the spatial resolution is not quite enough to do a
detailed analysis, but it is very useful to understand the severity of
storms hitting the island.


Weather station data
--------------------

Another good source of data is weather station data.  It is possible
to build a `DIY weather station`_ for a $200-300.  The project in the
link had some special constraints.  It was intented to create a
weather station that would show the conditions at a lake 2 hours drive
from the person that built it, so it needed to be robust against
system glitches.  

There are a number of weather stations here in Bermuda that are
connected to the `Weather Underground`_ network of stations.

Another project is `Open Weather Map`_.  This provides an API that you
can use to connect your weather station to the network.

For risk modelling purposes we ideally need historical data for the
times when the larger storms have hit the island.  The sites mentioned
above are primarily focussed on weather forecasting, rather than
collecting data for subsequent analysis, although they do also do
this.

Unfortunately, access to historical data is limited without a paid
subscription.  The sites have costs to cover, so small charges for
access to data is one way to continue to provide the service.

Full access to Open Weather Map historical data costs $2000 per
month.  If we want to create an environment where interested parties
can explore their ideas then removing these cost barriers is an
important step to take,

If Bermuda had a network of 100-200 weather stations it would open
lots of powerful modelling opportunities.  For example, machine
learning could be used to try and tease out the relationship between
weather station parameters such as height, distance from the coast,
local topography, land use and whatever other parameters are
available.

If such a model can be fitted to the data it can then be used to
estimate windspeed for any point on the island.  In this way we can
create a detailed windfield model for Bermuda.

Furthermore, most of the tools needed to do this are already available
as open source projects.  The pieces just need to be glued together.

Finally, any work done here in Bermuda can easily be generalised and
applied to other similar jurisdictions.


Damage surveys
++++++++++++++

If we also have a detailed, post event, damage survey we can also use
the same machine learning techniques to develop damage models relating
the hazard at each location to the damage it creates.

There are good open source tools, such as `scikit-learn`_ and
`scikit-image`_ that can be used for this modelling.

Humanitarian OpenStreetMap Team
+++++++++++++++++++++++++++++++

`Open Street Map`_ is an open mapping project that has been running
for many years::

    OpenStreetMap is built by a community of mappers that contribute and
    maintain data about roads, trails, cafes, railway stations, and much
    more, all over the world

The project has a number of related projects centred around the core
mapping project.

The `Humanitarian OpenStreetMap Team`_ works on mapping damage to help
with relief work following natural disasters, such as the recent Nepal
earthquakes. 

Whilst this work is focussed on disaster relief in the immediate
aftermath of a disaster it is producing valuable data which can be
used to better understand damage.  It could be a key input into new
models that can be used to explore mitigation measures for future
events. 

With the world facing unprecedented challenges, such as climate change
and increased earthquake risk due to human activities such as fracking
as well as the melting ice caps changing the stresses on tectonic
plates there is a humanitarian need to be able to model and explore
the potential impacts on delicate eco-systems such as small island
communities.

.. _Satellite mapping for everyone: https://www.youtube.com/embed/MCHpt1FvblI
.. _numpy: http://www.numpy.org/
.. _rasterio: https://github.com/mapbox/rasterio/
.. _Planet Labs: https//www.planet.com/
.. _Humanitarian OpenStreetMap Team: http://hotosm.org/
.. _Global Precipitation Measurement: http://pmm.nasa.gov/data-access/downloads/gpm
.. _DIY weather station: http://www.toptal.com/c/how-i-made-a-fully-functional-arduino-weather-station-for-300

.. _scikit-learn: http://scikit-learn.org/
.. _scikit-image: http://scikit-image.org/
.. _Open Street Map: https://www.openstreetmap.org/
.. _Weather Underground: http://weatherunderground.com
.. _Open Weather Map: http://openweathermap.org
.. _Gustave Dore: http://en.wikipedia.org/wiki/Gustave_Dor%C3%A9
.. _Wikimedia Commons: http://commons.wikimedia.org/wiki/

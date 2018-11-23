.. _index:

.. figure:: ./images/logo-180.png
    :alt: plotnine
    :align: right

A Grammar of Graphics for Python
================================

plotnine is an implementation of a *grammar of graphics* in Python.
It is based on ggplot2_. The grammar allows users to compose plots
by explicitly mapping data to the visual objects that make up the
plot.

Plotting with a grammar is powerful; it makes custom, 
complex plots easy to conceive and create, while keeping
simple plots simple.

Example
-------
.. code:: python

    (ggplot(mtcars, aes('wt', 'mpg', color='factor(gear)'))
     + geom_point()
     + stat_smooth(method='lm')
     + facet_wrap('~gear'))

.. figure:: ./images/readme-image-4.png

Documentation
-------------

.. toctree::
   :maxdepth: 1

   api
   installation
   gallery
   changelog
   about-plotnine
   tutorials
   glossary
   external-resources

.. _ggplot2: http://ggplot2.org

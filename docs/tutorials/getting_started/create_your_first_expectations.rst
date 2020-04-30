.. _getting_started__create_your_first_expectations:

Create your first Expectations
==============================

:ref:`Expectations` are the workhorse abstraction in Great Expectations.

The CLI will help you create your first Expectations. You can accept the defaults by typing [Enter] twice:

.. code-block:: bash

    Name the new expectation suite [religion-survey-results.warning]: 

    Great Expectations will choose a couple of columns and generate expectations about them
    to demonstrate some examples of assertions you can make about your data. 
        
    Press Enter to continue
    :

    Generating example Expectation Suite...

What just happened?
-------------------

You can create and edit Expectations using several different workflows. The CLI just used one of the quickest and simplest: scaffolding Expectations using an automated :ref:`Profiler`_.

This Profiler connected to your data (using the Datasource you configured in the previous step), took a quick look at the contents, and produced an initial set of Expectations. These Expectations are not intended to be very smart. Instead, the goal is to quickly provide some good examples, so that you're not starting from a blank slate when you begin.

Later, you should also take a look at other workflows for :ref:`creating and editing Expectations`_, such as:

    * :ref:`How to edit Expectations in a disposable notebook`
    * :ref:`How to adjust Expectations in a disposable notebook after Validation`
    * :ref:`How to profile many tables at once`
    * :ref:`How to calibrate Expectation Suite parameters using multibatch profiling`

The newly profiled Expectations are stored in an :ref:`Expectation Suite`. For now, they're stored in a JSON file in a subdirectory subdirectory of your ``great_expectations/`` folder. We'll take a look at the actual Expectations in the next step of the tutorial.

You can also configure Great Expectations to store Expectations to other locations, like S3, postgresql, etc. We'll come back to these options in the last step of the tutorial.

For now, let's continue to :ref:`Setting up data docs`.
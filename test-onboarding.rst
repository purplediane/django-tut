The Test Framework
==================

.. Estimated time: 3 minutes

Install Python
--------------

This class will be using Python 3. If you don't have Python 3 installed, please  visit the official `Python downloads page`_ and click the yellow "Download Python 3.8.2" button.

.. only:: html

    If you have any problems installing, please ask for help.


Download The Exercises
----------------------

Throughout this workshop we'll be using a test framework to check your code.  Here's what you need to know to make it all work.

.. only:: html

    Download :download:`exercise test files </files/exercises.zip>`.  When unzipped, it should create a new folder called ``exercises``. It contains the test framework we will be using, so you will be working from this folder.

.. only:: latex

    Download `exercise test files <https://pycon2018.trey.io/_downloads/0b8c992bd2f05a0da0466c853d48ffdb/exercises.zip>`_.  When unzipped, it should create a new folder called ``exercises``. It contains the test framework we will be using, so you will be working from this folder.

This file you downloaded (``exercises.zip``), when unzipped, should create a new folder called ``exercises``.
It contains the test framework we will be using, so you will be working from this folder.
It also contains the files you will need to modify for most of the exercises in the class.


Confirm the Framework is Working
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Change directory to your ``exercises`` directory, and run the following:

.. code-block:: bash

    $ python test.py is_ok

If successful, you'll receive this message:

.. code-block:: bash

    Testing is_ok

    Congrats and welcome to the Test Framework!
    The message confirms the Test Framework is working! Yay!
    Pat yourself on the back for successful installation!\n
    Continue reading this section of the course instructions. \n
    We will get started in a moment.
    .
    ----------------------------------------------------------------------
    Ran 1 test in 0.000s

    OK

To see what tests exist, you can also enter ``python test.py`` on the command line (or ``python3 test.py`` or ``py -3 test.py``) by itself:
You should see a list of lots of tests:

::

    Please select a thing to test

    iterators:

    first: Return the first item in given iterable.
    is_iterator: Return ``True`` if given iterable is an iterator.

    functions:

    around: Yield a tuple of the previous, current, and next items.
    deep_flatten: Flatten an iterable of iterables.
    pairwise: Yield a tuple containing each item and the item following it.
    stop_on: Yield from the iterable until the given value is reached.
    unique: Yield iterable elements in order, skipping duplicate values.
    ...


Where to Write Your Code
------------------------

At the beginning of each exercise you'll see a note describing where to find it.  The exercises will be functions you'll write or modify in the existing ``.py`` files in the ``exercises`` directory.  It's important that you write your code in the right place, or the tests won't work.


How to Run the Tests
--------------------

Once you've written your code and you're ready to test it, we will use Python to run ``test.py`` followed the name of the exercise in your command prompt.  Always type these commands from the ``exercises`` directory.  The test framework knows where to find the files you tell it to test.

How you run this at the terminal will depend on your operating system and which version(s) of Python you have installed.

If you only have one version of Python installed, and it is Python 3, you can run the tests (for example) for the ``get_vowel_names`` exercise in ``lists.py`` like this:

Linux/Mac terminal:

.. code-block:: bash

    $ python test.py get_vowel_names

Windows command window:

.. code-block:: bat

    > py test.py get_vowel_names

If you have more than one version of Python installed, you'll need to specify Python 3 like this:

Linux/Mac terminal:

.. code-block:: bash

    $ python3 test.py get_vowel_names

Windows command window:

.. code-block:: bat

    > py -3 test.py get_vowel_names

In all cases you should see a ``FAILED`` message at the end of the output, like this::

    Ran 3 tests in 0.000s

    FAILED (errors=3)

Your tests **should** be failing at first because you haven't written any code to get them to pass yet!


Passing the Tests
-----------------

Once you've attempted the exercise by adding code to the ``get_vowel_names`` function in ``lists.py``, if your code has passed the tests, you'll see some variation of this message:

::

    Testing get_vowel_names

    ...
    ----------------------------------------------------------------------
    Ran 3 tests in 0.002s

    OK


.. _Python downloads page: https://www.python.org/downloads/

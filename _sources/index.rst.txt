.. Boilerplate documentation master file, created by
   Ho2eny on Thu Apr 14 15:23:01 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to documentation! 
========================== 

Boilerplate that deploys reStructuredText docs to Github Page 

Build the docs
--------------- 

**Install Sphinx and Theme**

::

  pip install -r requirements.txt

**Building the docs**

In the ``docs/`` folder ::

  make html

If you want to building each time a file is changed ::

  sphinx-autobuild . _build/html

Deploys docs with Github Pages
-------------------------------

When you push some ``.rst`` documents to ``master``, **Github Action** builds sphinx and deploys static html to ``gh-pages`` branch.

You can publish the ``gh-pages`` branch on **Github Pages**

Set the **Github Pages** source to ``gh-pages`` ``/(root)`` in the repository **Settings**

.. toctree::
   :maxdepth: 1
   :caption: Template_1

   Template_1/sample_page

.. toctree::
   :maxdepth: 1
   :caption: Template_2

   Template_2/sample_page_2

Indices and tables 
================== 

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

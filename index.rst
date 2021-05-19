..
  Technote content.

  See https://developer.lsst.io/restructuredtext/style.html
  for a guide to reStructuredText writing.

  Do not put the title, authors or other metadata in this document;
  those are automatically added.

  Use the following syntax for sections:

  Sections
  ========

  and

  Subsections
  -----------

  and

  Subsubsections
  ^^^^^^^^^^^^^^

  To add images, add the image file (png, svg or jpeg preferred) to the
  _static/ directory. The reST syntax for adding the image is

  .. figure:: /_static/filename.ext
     :name: fig-label

     Caption text.

   Run: ``make html`` and ``open _build/html/index.html`` to preview your work.
   See the README at https://github.com/lsst-sqre/lsst-technote-bootstrap or
   this repo's README for more info.

   Feel free to delete this instructional comment.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This is a SQuaRE delivery note covering the web forum service deployed as community.lsst.org and related infrastructure.**

   A delivery note is being used to transition a service (or other codebase) from Rubin Construction to Operations in situations where the service is not covered by a requirements document, is not part of the observatory operational readiness milestone, or otherwise lacks a formal process of delivery.

   Its purpose is to document the transition so as to allow Ops-funded developers to continue to maintain and evolve the service, and to allow the service's deployment costs to be covered by Ops infrastructure or funding. It can also be used to describe responsibilities for the service when not a direct continuation of the model used in construction. 

.. Add content here.

What is covered
===============


What artifacts (code, docs) are involved?
-----------------------------------------

What costs does the service incurr?
-----------------------------------


Responsibilities
================

What construction team is delivering the service?
-------------------------------------------------

What operations team is receiving the service?
----------------------------------------------

What differences should one expect post-transition?
---------------------------------------------------



   
.. Do not include the document title (it's automatically added from metadata.yaml).


   
.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa

..
  Technote content.

:tocdepth: 1

.. Please do not modify tocdepth; will be fixed when a new Sphinx theme is shipped.

.. sectnum::

.. TODO: Delete the note below before merging new content to the master branch.

.. note::

   **This is a SQuaRE delivery note covering the web forum service deployed as community.lsst.org and related infrastructure.**

   A Delivery Note is being used to transition a service (or other codebase) from Rubin Construction to Operations in situations where the service is not covered by a requirements document, is not part of the observatory operational readiness milestone, or otherwise lacks a formal process of delivery.

   Its purpose is to document the transition so as to allow Ops-funded developers to continue to maintain and evolve the service, and to allow the service's deployment costs to be covered by Ops infrastructure or funding. It can also be used to describe responsibilities for the service when not a direct continuation of the model used in construction.

   The process is complete when the relevant AD(s) and/or Director reviews the note and the note is published (merged to master).

   **Reviewed by:** Wil O'Mullane and Bob Blum

.. Add content here.

Scope
=====

This delivery note covers the Discourse-based web forum service deployed as community.lsst.org

The web forum is a destination for long-lived (compared to Slack) discussion forum replacing mailing lists for internal project use, as well as a community-facing forum designed to involve the community in discussions with the project as well as their peers in an asynchronous and searchable manner.

Artifacts (code, docs, infrastructure) involved in this delivery
----------------------------------------------------------------

The following repositories include visual (theme) styling components:

- https://github.com/lsst-sqre/discourse-rubin-theme
- https://github.com/lsst-sqre/discourse-alt-lock-icon
- https://github.com/lsst-sqre/discourse-rubin-header
- https://github.com/lsst-sqre/discourse-rubin-footer

The following repo documents an example of how to use the Discourse API:

- https://github.com/lsst-sqre/community_api

Additionally the following resources are involved in the operation of this service:

- DigitalOcean droplet
- Mailchimp account for email
- Let's Encrypt account for TLS
- AWS S3 bucket for backups
- Slack application to bridge Discourse and Slack
- Twitter app for OAuth login
- GitHub OAuth app for login
- 1Password for secrets management

The motivation for the service's creation and outline of its elements can be found at https://sqr-011.lsst.io/#community-forum-and-mailing-lists

Potential costs
---------------

The service is hosted on a Digital Ocean droplet and costs approximately $30/month billed directly to an AURA Purchasing credit card under a blanket PO against CS008.1.02C.10.01.KLM21001A. A new PO will be issued for Operations under CS002.

Ongoing support
---------------

The slack channel #rubinobs-forum-team offers support of and discussion with content administators of the forum, such as the Ops Community Engagement Team.

Users of the forum can discuss management issues of the forum on the forum itself under the Meta category: https://community.lsst.org/c/meta/3


Handover
========

Delivering team
----------------

SQuaRE built and operates this service during Construction on behalf of Data Management.

As a project forum, content was contributed organically primarily by project staff.

Receiving Operations team
--------------------------

In Operations, community.lsst.org is a collaboration between SQuaRE (DPP) and CET (RPF)

SQuaRE will continue operating the service during Operations on behalf of Data Production.
This includes all technical aspects of operating the service including its deployment, technical and design upgrades as well as security updates, backups, etc.

The Community Engagement Team will be responsible for content management of the sections of the forum accessible to the Rubin Scientific Community on behalf of Rubin System Performance.
It is also responsible for setting policy in areas that are relevant to its activities, eg. what the protocol is for answering user questions.

The teams use the Slack channel #rubinobs-forum-team to communicate intended work, discuss improvements and genereally keep the other informed.

Authorization or asset transfer
-------------------------------

No authorisation information is required.

SQuaRE maintains the administrative secrets required to operate the service.
Select members of CET have full adminstrative rights on the forum itself.

Known Issues
============

There are no known issues with the service.

Development on this service is largely reactive driven by user and content-administrator requests.

For billing efficiency, we may wish to consider at some point in the future deploying the service on our main cloud services provider in the future, as it is one of only two SQuaRE services hosted on Digital Ocean for historical reasons.

Additional Notes
================

DNS
---
As the service is deployed under the lsst.org domain controlled by (in Construction) Project IT, co-ordination is required with that group or its successor for any DNS changes.

Visual Identity
---------------
The theming elements of the forum use assets from the visual identity guide and the visual identity style dictionary. Co-ordination is required with the Rubin visual identity team.


.. Do not include the document title (it's automatically added from metadata.yaml).



.. .. rubric:: References

.. Make in-text citations with: :cite:`bibkey`.

.. .. bibliography:: local.bib lsstbib/books.bib lsstbib/lsst.bib lsstbib/lsst-dm.bib lsstbib/refs.bib lsstbib/refs_ads.bib
..    :style: lsst_aa

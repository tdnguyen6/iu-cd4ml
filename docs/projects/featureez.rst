**********
featureez
**********

This page host the documentation for **featureez** project.

----------------------------------

.. contents:: Table of Contents
    :local:

----------------------------------

Product Backlog
===============

.. list-table:: Product backlog table
    :widths: 5 5 80 10
    :header-rows: 1
    :stub-columns: 1

    * - Id
      - Story
      - Task 
      - Status
    * - 1
      - n/a
      - Set up project structure 
      - 


User stories
=============

.. list-table:: User stories table
    :widths: 2 2 6 45 45
    :header-rows: 1
    :stub-columns: 1
    
    * - Id
      - Point(s)
      - As a(n)
      - I want to (be able to)
      - so that (I can)
    * - 1
      - 1
      - featureez host
      - have lazy evaluation for features
      - | save storage in the long term
        | especially when I have to support
        | multiple feature versions
    * - 2
      - 5
      - feature user
      - have a UI
      - see:

        * catalog
        * validation
        * version
        * etc.

        and other info related to a feature
    * - 3
      - 3
      - feature user
      - have feature versioning
      - use old features
    * - 4
      - 3
      - feature user
      - have point-in-time joining of features
      - have time-compatible feature dataframe
    * - 5
      - 1 
      - feature user
      - see the feature engineering code
      - | understand feature engineering
        | logic easily and modify to create
        | my own features if I want
    * - 6
      - 8
      - feature user
      - see the feature validation
      - know feature quality
    * - 7
      - 13
      - feature user
      - see the feature dependency hierarchy
      - understand features relationships
    * - 8
      - 8
      - feature user
      - estimate feature delivery time
      - estimate the time in my use case
    * - 9
      - 8
      - ML scientist
      - get feature on-demand
      - serve my model with online prediction
    * - 10
      - 8 
      - feature developer and user
      - have multi-lingual support
      - develop and use feature in any language
    * - 11
      - 8
      - feature developer and user
      - notify when features change
      - take necessary actions for each change
    * - 12
      - 13
      - feature user and developer
      - diff feature between versions
      - | see how feature changes. In case of 
        | updating manual features, I want to
        | update my feature only for entities
        | with changed dependencies
    * - 13
      - 1 
      - feature developer
      - have an SDK with CI/CD
      - develop feature easily
    * - 14
      - 5
      - feature developer
      - create features manually (row by row)
      - | provide mannually collected features
        | like ML labels 
    * - 15
      - 5
      - feature developer
      - | update feature automatically based
        | on my logic
      - features are up to date
    * - 16
      - 5
      - feature developer
      - have dependencies as other features
      - reused other features in my transformer
    * - 17
      - 5
      - feature developer
      - set authorization rules for my feature
      - limit access to my feature
    * - 18
      - 5
      - enterprise featureez host
      - host my own featureez on-prem or on-cloud
      - ensure the confidentiality of my data


Framework Stack of choice
=========================

featureez server
----------------

Web stack:

* Django
* Vuejs
* Tailwindcss

Anemoi client
-------------

Tools:

* Python
* Airflow


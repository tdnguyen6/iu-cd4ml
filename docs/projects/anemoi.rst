***********
anemoi
***********

This page host the documentation for **anemoi** project.

----------------------------------

.. contents:: Table of Contents
    :local:

----------------------------------


User stories
=============

Story Table
-----------

.. list-table:: User stories table
    :widths: 2 8 45 45
    :header-rows: 1
    :stub-columns: 1
    
    * - Id
      - As a(n)
      - I want to (be able to)
      - so that (I can)
    * - 1
      - airflow user
      - be able to export DAGs
      - share it with other people
    * - 2
      - airflow user
      - be able to import DAGs
      - reuse DAGs from other people
    * - 3
      - anemoi user
      - search for DAGs on anemoi UI
      - easily discover DAGs relevant to me
    * - 4
      - anemoi user
      - visual DAGs on anemoi UI
      - know the basic flows of the DAGs
    * - 5
      - anemoi user
      - apply below filters to searched DAGs:

        * label
        * upvotes
        * ratings
        * tags
        * categories
        * user
        * airflow version
        * executors type
        * operators type
      - | give more specific requirements
        | about the DAGs that I need
    * - 6
      - anemoi user
      - | quickly find out basic info of
        | searched DAGs like:

        * DAG version
        * airflow version
        * executors type
        * operators type
        * input
        * output
        * xcoms (shared data)
        * schedule
        * system requirements:
            
          * Memory
          * CPU
          * Diskspace
          * Network
      - Immediately know if a DAG is suitable
    * - 7
      - anemoi user
      - | upvote a useful DAGs
        | downvote a useless DAGs
      - | leave hints about how useful
        | each DAG is for other users
    * - 8
      - anemoi user
      - rate and comment on a DAG
      - | express my opinion and experience
        | after on a DAG
    * - 9
      - anemoi user
      - authenticate me on anemoi
      - | do other things within anemoi
        | as an authorized user
    * - 10
      - anemoi user
      - limit the access scope of my DAG
      - share DAGs only to the people I want
    * - 11
      - anemoi user
      - | update my DAG on anemoi
        | with newer versions
      - make sure my DAG has no issue
    * - 12
      - anemoi user
      - fork another user's DAG
      - | improve other user's DAG
        | or provide new feature
        | for that DAG. For example,
        | provide a different DAG
        | version that can use another
        | executor type
    * - 13
      - anemoi user
      - | compare DAGs across 
        | versions and forks
      - | know which version or fork
        | of a DAG to choose
    * - 14
      - anemoi user
      - | set parameters on my
        | exported DAG
      - | people who import my DAG
        | can easily customize it
        | to their needs

Story Execution
---------------

.. list-table:: Stories execution table
    :widths: 1 9 10 20 60
    :header-rows: 1
    :stub-columns: 1

    * - Id
      - Point(s)
      - sprint no.
      - Status
      - Remark
    * - 1
      - 8
      - TBD
      - new
      - 
    * - 2
      - 8
      - TBD
      - new
      - 
    * - 3
      - 3
      - TBD
      - new
      - 
    * - 4
      - 13
      - TBD
      - new
      - 
    * - 5
      - 3
      - TBD
      - new
      - 
    * - 6
      - 3
      - TBD
      - new
      - 
    * - 7
      - 3
      - TBD
      - new
      - 
    * - 8
      - 3
      - TBD
      - new
      - 
    * - 9
      - 1
      - 1
      - in progress
      - 
    * - 10
      - 3
      - TBD
      - new
      - 
    * - 11
      - 3
      - TBD
      - new
      - 
    * - 12
      - 5 
      - TBD
      - new
      - 
    * - 13
      - 21
      - TBD
      - new
      - 
    * - 14
      - 5
      - TBD
      - new
      - 

Framework Stack of choice
=========================

Anemoi server
-------------
Web stack:

* Django
* Vuejs
* Tailwindcss

Anemoi client
-------------

Tools:

* Python
* Airflow

Direction: develop as an airflow plugin

.. Introduction
.. ============

.. Motivation
.. ----------

.. Problem statement
.. -----------------

.. Scope
.. -----

.. Literature Review
.. ======================

.. Similar systems
.. ---------------

.. Review similar systems
.. ----------------------

.. Requirement Analysis
.. ====================

.. User stories
.. ------------

.. Usecase Descriptions
.. --------------------

.. Functional requirements
.. -----------------------

.. Non-functional requirements
.. ---------------------------

.. System Design
.. ======================

.. Packages and Modules
.. --------------------

.. Tools and Techniques
.. --------------------

.. Diagrams
.. ---------

.. Usecase Diagram
.. ^^^^^^^^^^^^^^^

.. Sequence Diagrams
.. ^^^^^^^^^^^^^^^^^^^^

.. Activity Diagrams
.. ^^^^^^^^^^^^^^^^^^^^

.. E-R Diagrams
.. ^^^^^^^^^^^^^^^^^^^^

.. Class Diagrams
.. ^^^^^^^^^^^^^^^^^^^


.. System Implementations
.. ======================

.. Sprint 1
.. ---------

.. Sprint 2
.. ---------

.. Anemoi Progress
.. =======================

.. Problems anemoi solved
.. --------------------------

.. Problems anemoi yet to solve
.. --------------------------------

.. anemoi compared to other systems
.. -------------------------------------

.. Future roadmap of anemoi
.. ----------------------------

.. References
.. =======================

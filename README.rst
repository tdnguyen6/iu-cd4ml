###############
CD4ML - MLOps
###############

.. image:: https://readthedocs.org/projects/iu-cd4ml/badge/?version=latest
    :target: https://iu-cd4ml.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status

This is the documentation for all my projects in CD4ML field for Bachelor's thesis at International University 2021-2022

Read the complete documentation at: `iu-cd4ml.readthedocs.io <https://iu-cd4ml.readthedocs.io>`_

----------------------------------

.. contents:: Table of Contents
    :local:

----------------------------------

***********
Overview
***********
In Software Engineering, DevOps and Continuous Delivery has become an integral part as it did a great job automating the boring parts of the SE process. The more complicated the project, the more useful DevOps is. Popular software platforms also provided extensive supports for CI/CD with GitHub Actions, or even the whole DevOps lifecycle with GitLab.

Machine learning is an emerging but attractive field as ML can bring solutions to problems beyond the SE ability. Having realized the immense value of DevOps in Software Engineering, ML experts are calling for an adaptation of CI/CD pipelines to the ML field in order to streamline the process between ML development and deploying ML in production, naming the new field CD4ML or MLOps. Nevertheless, due to some instrinsical differences between ML and SE, MLOps faced a lot of obstables. Some of the perks of ML include: probabilistic nature, non-deterministic results, heavy reliant on data (which is hard to manage), non-code backgrounds of ML practitioners, etc.

***************
Vision & Ideas
***************

Visions
=======

In my thesis, I set out to solve some of the current problems faced by MLOps systems.

A new concept has been created in ML systems in order to reduce the duplicated work between ML teams and projects, that is **feature store**. Feature store is like a data warehouse, but focus specifically on storing ML features (columns after doing feature engineering on datasets). As data scientists are currently spending the majority of time on feature engineering, if the feature engineering work can be shared and reused by other teams or projects, it would boost the productivity of data scientists many times.

There are a lot of featurestore solutions currently existing. Nevertheless, most of them are proprietary and are deployed within the scope of the organizations. There are many reasons for this, most of those surrounds three aspects: infrastructure, data and incentives. Firstly, featurestore comes hand in hand with ETL pipelines, but ETL pipelines solutions are now still very customized to each organiztion's infrastructure, not portable enough to release in an open-source solution. Secondly, data comes in every shapes and sizes, thus, it is hard to release an open-source solution that can fit every system's data. Reversely, organizations decided to better design a customized featurestore that support well the kind of data frequently appeared inside of their organizations. Last but not least, organizations do not have an incentive to develop, release and maintian an open-source featurestore. The only open-source featurestore as of now, late 2021, is Feast, developed by Tecton and used internally by Gojek.

Here is a comparison of featurestores from `featurestore.org <https://featurestore.org>`_:

.. figure:: docs/_static/featurestore-compare.png

    Feature store comparison table.

As the only available open-source featurestore, Feast gain traction easily. However, Feast is kind of a low-priority project for the maintaining organizations. Despite being developed for almost 3 years, it is still very basic, lacking a lot of features. Even feast admitted that they lack some crucial features, taken from `docs.feast.dev <https://docs.feast.dev>`_:

.. figure:: docs/_static/feast-problems.png

    Feast problems.

Besides, there are other problems that I found after having used feast for a while:

* Only support time-series data. Many teams has requested them to support other kinds of data, especially for datasets without timestamps
* Tightly coupled to Gojek workflow:

  #. Gathering timestamped data
  #. Do feature engineering and store features in offline store
  #. Schedule job to move newest (usually within last 24 hours) rows of features from offline store to online store
  #. Label and train model on features in offline store
  #. Use trained model to predict labels of newest features in online store

* Many projects that have workflows requiring on-demand inferences will not fit into Feast design.
* No guarantee between the feature and its feature engineering pipelines. When feature users and feature engineers are from 2 different teams (which is one of the originial goals of feature stores, sharing features between teams and projects), features users will not be guaranteed to know about the feature engineering logics:

  #. who are the feature engineers for a feature?
  #. what techniques, sources, etc. created that feature?
  #. when was that feature first appeared, when is it scheduled to update, to materialize?
  #. how was the feature engineered, aka what is its logic? how to update the feature?
  #. why was that feature created, what was the purpose of it or why doesn't a crucial feature exist in the feature store?


Due to all the reasons above, Feast, despite being popular, is being adopted very slowly, usually by teams that have data fit into Feast workflow and allow to spend time on customizing Feast. Three years in existence, even as the only choice for feature store, Feast only has 2.1k stars on GitHub.


featureez
=========

**featureez** is a next-generation feature store, completely open source, supporting a lot of advanced features compared to the currently existing feature store solutions like **feast**. 

The design of **featureez** does not have much in common to other feature stores, it hopes to bring a new perspective to the current feature store paradigm.

As an open source solution, **featureez** expects to become the go to feature store for the community. If **featureez** is widely adopted by the community, it can create an explosion in feature engineering and in machine learning in general due to the ability to share and reuse features with each other.

e2e-ml
======

This is simply an Electron app using different :code:`BrowserView` components to render MLOps tools in an ML life cycle. For example, one view for AirFlow, one for a Feature Store and another view for a Metadata Store.

The purpose of this project is to showcase the enhancements that MLOps can bring to the ML lifecycle.

***********
Resources
***********

Time
=====

.. list-table:: Deadlines
    :widths: 25 25
    :header-rows: 1
    
    * - Purpose
      - Date
    * - Implementations
      - November 2021
    * - Thesis Defend
      - ~ February 2022

Human
=====

.. list-table:: Human Resources
    :widths: 25 25 50
    :header-rows: 1

    * - Role
      - Quantity
      - Name(s)
    * - Student
      - 1
      - Nguyen Tien Duc
    * - Instructor/Mentor
      - 1
      - Dr. Tran Thanh Tung

***********
References
***********
TBD.




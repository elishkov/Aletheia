======================
Aletheia
======================

.. image:: ../logo/Aletheia-logo.png

What is Aletheia?
---------------------
Large scale environments tend to have streams of incoming data, which need to be routed to multiple destinations. For instance, data may need to be written to log files that are to be consumed and loaded to a Hadoop cluster for batch oriented processing, as well as sent to Kafka to be consumed a real-time computation framework.
Creating a production grade and robust data pipeline involves many challenges, some of which we list below. 
Aletheia is a new data delivery framework that aims to address these challenges.

Uniform and Extendable API
--------------------------
Aletheia provides a uniform API to interface with multiple destination endpoints. The endpoint model is fully pluggable, supporting Kafka and log files out-of-the-box and allowing to create new endpoint types easily. Aletheia supports both built-in and custom serialization formats, and sets the foundation for supporting schema evolution in the future.

Visibility
--------------------------
Fine grained monitoring and visibility is one of one of Aletheia’s main concerns. This is achieved by a mechanism called Breadcrumbs. Breadcrumbs are pieces of metadata that are calculated over short time windows by each producer and consumer along the pipeline. This metadata contains information such as source, destination and aggregated counts. Breadcrumbs are periodically sent to a destination of choice by each producer and consumer, allowing near real-time analysis by a monitoring authority.


Contents
--------

.. toctree::
    :maxdepth: 2

    Getting Started 
    Related Reading 

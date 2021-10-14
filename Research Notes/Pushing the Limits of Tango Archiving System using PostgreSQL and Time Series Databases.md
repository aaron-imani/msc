# Pushing the Limits of Tango Archiving System using PostgreSQL and Time Series Databases
## Paper Link

https://accelconf.web.cern.ch/icalepcs2019/papers/wepha020.pdf

## Research Questions

- How different the performance of different back-ends and the extension of HDB++ is to support TimescaleDB for insertion and extraction?

## Brief Summary

This study makes a comparison between the different supported database backends for Tango archiving system, HDB++. The supported database backends which are MySQL/MariaDB, Cassandra, PostgreSQL, TimescaleDB, and Elasticsearch have been compared using `hdbpp-metrics` Github repository benchmarking tools. According to their results:
- The new PostgreSQL and TimescaleDB backends improve the user experience when dealing with Tango spectrum (array) attributes.
- Cassandra back-end is currently a good fit for use cases where high availability is required for writing the archiving data and where scalar attributes data has to be stored. It is not a good fit for retrieving big chunks of data, in particular for getting multi-dimensional data.
- The Elasticsearch backend is a good fit for users interested in benefiting from the advantages of the ELK stack.

## Findings

-  Presents the benchmarking tools that have been developed to compare the performance of different back-ends and the extension of HDB++ to support TimescaleDB for insertion and extraction.
-  A comparison of the different supported back-ends
  
## Suggested Future Work

None
  
## Relevance to my work

They have tried to push the limits of Tango Control in some aspect (HDB++)


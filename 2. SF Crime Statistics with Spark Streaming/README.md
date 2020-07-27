# SF Crime Statistics with Spark Streaming

## Project Overview

In this project, with the provided a real-world dataset, extracted from Kaggle, on San Francisco crime incidents, you will provide statistical analyses of the data using Apache Spark Structured Streaming. You will draw on the skills and knowledge you've learned in this course to create a Kafka server to produce data, and ingest data through Spark Structured Streaming.

## Development Environment

You may choose to create your project in the workspace we provide here, or if you wish to develop your project locally, you will need to set up your environment properly as described below:

  * Spark 2.4.3
  * Scala 2.11.x
  * Java 1.8.x
  * Kafka build with Scala 2.11.x
  * Python 3.6.x or 3.7.x
  
## Q1. How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

* Affects `processedRowsPerSecond`

## Q2. What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

* When using the default values, `processedRowsPerSecond` is about 30.
However, when using `maxOffsetPerTrigger` as 5000, `processedRowsPerSecond` is about 40.

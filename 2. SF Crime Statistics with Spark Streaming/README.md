# Udacity--Data-Streaming-project-2


## Q1. How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

* Affects `processedRowsPerSecond`

## Q2. What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

* When using the default values, `processedRowsPerSecond` is about 30.
However, when using `maxOffsetPerTrigger` as 5000, `processedRowsPerSecond` is about 40.

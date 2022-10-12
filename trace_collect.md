# trace collect
## Sample Rate
## mq producer
mq produce should support an env variable, named `TRACE_SAMPLE_RATE`, range from 0 to 1
## trace collect metadata
- isSample: detect a span should be collected
- traceId: trace id
- spanId: span id
## metadata in pulsar
Put the metadata in pulsar headers
# Support Data Exporters
## MongoDB
### TableName
trace_collect
### TableField
- traceId
- spanId

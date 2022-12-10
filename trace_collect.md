# trace collect
## Sample Rate
## mq producer
mq produce should support an env variable, named `TRACE_SAMPLE_RATE`, range from 0 to 1
## trace collect metadata
- isSample: detect a span should be collected
- traceId: trace id
- spanId: span id
- parenSpanId: parent span id
- component:
    - HTTP-SERVER
    - PULSAR-PRODUCER
    - PULSAR-CONSUMER
- startTime: starting time
- endTime: end time
- uri: 
    - http: uri
    - pulsar: topic
- method:
    - http: method
    - pulsar : CONSUMER/PRODUCER
## trace transfer
### header name
- perf-trace-id
- perf-span-id
### header position
- http:header
- pulsar:properties
## metadata in pulsar
Put the metadata in pulsar headers
# Support Data Exporters
## MongoDB
### TableName
trace_collect
### TableField
- traceId
- spanId

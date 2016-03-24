# 3.0.2
  - Depend on logstash-core-plugin-api instead of logstash-core, removing the need to mass update plugins on major releases of logstash
# 3.0.1
  - New dependency requirements for logstash-core for the 5.0 release
## 3.0.0
 - Elasticsearch 2.0 does not allow field names with dots in them.  This is a
   breaking change which replaces the `.` with an underscore, `_`

## 2.0.0
 - Plugins were updated to follow the new shutdown semantic, this mainly allows Logstash to instruct input plugins to terminate gracefully,
   instead of using Thread.raise on the plugins' threads. Ref: https://github.com/elastic/logstash/pull/3895
 - Dependency on logstash-core update to 2.0

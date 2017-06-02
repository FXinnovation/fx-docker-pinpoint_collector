# pinpoint-collector 
[![](https://images.microbadger.com/badges/version/fxinnovation/pinpoint-collector.svg)](https://microbadger.com/images/fxinnovation/pinpoint-collector "Get your own version badge on microbadger.com") [![](https://images.microbadger.com/badges/image/fxinnovation/pinpoint-collector.svg)](https://microbadger.com/images/fxinnovation/pinpoint-collector "Get your own image badge on microbadger.com")
## Description
This image contains pinpoint-collector. The image is based on the official alpine openjdk image. It should be more lightweight this way.

## Tags
We do NOT push a `latest` tag for this image. You should always pin a specific version for it.
We do not follow the pinpoint-collector release tags in the docker image tags. You can always find the pinpoint-collector version in the Dockerfile that was used to create the image or you can use the labels.

## Usage
```
docker run --rm -it -e [KEY]=[VALUE] fxinnovation/pinpoint-collector:[TAG]
```
Here is the list of keys you can set:

| Key | Default Value |
|-----|:-------------:|
| HBASE_CLIENT_HOST | localhost |
| HBASE_CLIENT_PORT | 2181 |
| HBASE_ZOOKEEPER_ZNODE_PARENT | "/hbase" |
| HBASE_IPC_CLIENT_TCPNODEDELAY | "true" |
| HBASE_RPC_TIMEOUT | 10000 |
| HBASE_CLIENT_OPERATION_TIMEOUT | 10000 |
| HBASE_IPC_CLIENT_SOCKET_TIMEOUT_READ | 20000 |
| HBASE_IPC_CLIENT_SOCKET_TIMEOUT_WRITE | 60000 |
| HBASE_CLIENT_THREAD_MAX | 64 |
| HBASE_CLIENT_THREADPOOL_QUEUESIZE | 10000 |
| HBASE_CLIENT_THREADPOOL_PRESTART | "false" |
| HBASE_CLIENT_ASYNC_ENABLE | "false" |
| HBASE_CLIENT_ASYNC_IN_QUEUESIZE | 1000 |
| HBASE_CLIENT_ASYNC_FLUSH_PERIOD_MS | 100 |
| HBASE_CLIENT_ASYNC_MAX_RETRIES_IN_QUEUE | 10 |
| COLLECTOR_TCPLISTENIP | 0.0.0.0 |
| COLLECTOR_TCPLISTENPORT | 9994 |
| COLLECTOR_TCPWORKERTHREAD | 8 |
| COLLECTOR_TCPWORKERQUEUESIZE | 1024 |
| COLLECTOR_WORKER_MONITOR | "true" |
| COLLECTOR_UDPSTATLISTENIP | 0.0.0.0 |
| COLLECTOR_UDPSTATLISTENPORT | 9995 |
| COLLECTOR_L4_IP | "" |
| COLLECTOR_UDPSTATWORKERTHREAD | 8 |
| COLLECTOR_UDPSTATWORKERQUEUESIZE | 64 |
| COLLECTOR_UDPSTATWORKER_MONITOR | "true" |
| COLLECTOR_UDPSTATSOCKETRECEIVEBUFFERSIZE | 4194304 |
| COLLECTOR_UDPSPANLISTENIP | 0.0.0.0 |
| COLLECTOR_UDPSPANLISTENPORT | 9996 |
| COLLECTOR_UDPSPANWORKERTHREAD | 32 |
| COLLECTOR_UDPSPANWORKERQUEUESIZE | 256 |
| COLLECTOR_UDPSPANWORKER_MONITOR | "true" |
| COLLECTOR_UDPSPANSOCKETRECEIVEBUFFERSIZE | 4194304 |
| COLLECTOR_AGENTEVENTWORKER_THREADSIZE | 4 |
| COLLECTOR_AGENTEVENTWORKER_QUEUESIZE | 1024 |
| STATISTICS_FLUSHPERIOD | 1000 |
| CLUSTER_ENABLE | "true" |
| CLUSTER_ZOOKEEPER_ADDRESS | localhost |
| CLUSTER_ZOOKEEPER_SESSIONTIMEOUT | 30000 |
| CLUSTER_LISTEN_IP | "" |
| CLUSTER_LISTEN_PORT | "" |
| COLLECTOR_SPANEVENT_SEQUENCE_LIMIT | 10000 |
| COLLECTOR_SPAN_FORMAT_COMPATIBILITY_VERSION | v2 |
| COLLECTOR_STAT_FORMAT_COMPATIBILITY_VERSION | v2 |

## Labels
We set labels on our images with additional information on the image. we follow the guidelines defined at http://label-schema.org/. Visit their website for more information about those labels.

## Comments & Issues
If you have comments or detect an issue, please be advised we don't check the docker hub comments. You can always contact us through the repository.

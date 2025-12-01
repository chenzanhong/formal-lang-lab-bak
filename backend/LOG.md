# 日志消费（待规划与实现）
使用Filebeat收集日志，Kafka作为消息中间件，go-stash处理日志，最终存储到Elasticsearch，通过Kibana进行可视化查询。

## 架构
```
[AI/Auth/Email/Master 服务]
        ↓ (写本地文件)
     ./logs/*.log
        ↓
    Filebeat（轻量 Shipper）
        ↓
      Kafka（缓冲 + 解耦）
        ↓
   go-stash（日志处理/解析/过滤）
        ↓
 Elasticsearch（存储 + 索引）
        ↓
    Kibana（可视化）
```
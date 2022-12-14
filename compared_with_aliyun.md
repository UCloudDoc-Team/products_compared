# 与阿里云对比

| **阿里产品**                  | **UCloud对应产品** | **满足度**                                                   | **差异**                                                     |
| ----------------------------- | ---------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ECS + 云盘                    | 快杰+UDisk             | 完全满足                                                     |                                                              |
| 弹性裸金属服务器              | 裸金属                 | 完全满足                                                     |                                                              |
| Mysql、PG、sqlServer、mongoDB | UDB                    | 完全满足                                                     |                                                              |
| memcache、redis               | UMem                   | 完全满足                                                     |                                                              |
| PolarDB                       | TiDB                   | 部分满足：使用pdb专有特性的场景例外;核心需求是兼容MySQL,应对海量存储和高并发业务 | PolarDB与TiDB架构不一样,PolarDB是一主多从架构,单机写入也有性能瓶颈,TiDB是分布式数据库; PolarDB-X与TiDB架构一致,功能完全满足,但PolarDB-X企业版采用共享存储,秒级扩容计算节点,TiDB官方目前还不支持共享存储 |
| 数据传输服务 DTS              | UDTS                   | 完全满足                                                     |                                                              |
| 对象存储oss                   | US3                    | 完全满足                                                     |                                                              |
| 检索分析服务Es                | ES（开源版）           | 部分满足：必须使用企业版的除外                               | 我们没有X-Pack高级特性(1.对索引和字段实现分权管理,控制访问权限 2.数据监控,自动预警和上报告警 3.多维度(集群、节点、索引)监控 4.与传统SQL对接) |
| 文件存储NAS                   | UFS                    | 大部分满足:我们暂不支持SMB协议、ACL、数据加密                |                                                              |
| 内容安全lvwang                | 无                     | 不满足                                                       |                                                              |
| 云安全中心                    | 云安全中心             | 完全满足                                                     |                                                              |
| Web应用防火墙waf              | UWAF                   | 完全满足                                                     |                                                              |
| DDOS防护                      | 高防UDdos              | 完全满足                                                     |                                                              |
| 高速通道                      | UDPN                   | 完全满足                                                     |                                                              |
| NAT网关                       | NAT网关                | 完全满足                                                     |                                                              |
| CDN                           | CDN                    | 完全满足                                                     |                                                              |
| 负载均衡                      | ULB                    | 完全满足                                                     |                                                              |
| 全球加速                      | PathX                  | 完全满足                                                     |                                                              |
| 任播弹性公网IP                | AnycastEIP             | 完全满足                                                     |                                                              |
| 全站加速                      | 无                     | 不满足:动态+静态加速                                         |                                                              |
| VPN网关                       | IPSecVPN               | 部分满足:我们只有IPSecVPN连接,没有SSL-VPN连接                |                                                              |
| 边缘计算EBS                   | UEC-VM                 | 部分满足:只有部分三通机房节点                                |                                                              |
| 云解析PrivateZone             | UDNS                   | 完全满足                                                     |                                                              |
| Kafka                         | UKafka                 | 完全满足                                                     |                                                              |
| 日志服务sls                   | 无                     | 核心需求是低成本存储和查询，可用presto+us3 替换              |                                                              |
| 云监控cms                     | 无                     | 不满足                                                       |                                                              |
| 弹性伸缩                      | 无                     | 不满足                                                       |                                                              |
| TableStore                    | 无                     | 不满足                                                       |                                                              |
| OpenSearch                    | 无                     | 核心需求是将数据库中数据实时同步到搜索引擎进行词组查询,可用ES+LogStash或者ES+Canal替代 |                                                              |
| Serverless应用引擎            | UKubernetes            | 核心需求是免运维Iaas,实现资源编排,急速弹性伸缩,节约成本      |                                                              |
| 开源大数据平台E-MapReduce     | UHadoop                | 完全满足                                                     |                                                              |
| 云数据库ClickHouse            | ClickHouse             | 完全满足,架构同社区兼容版                                    |                                                              |

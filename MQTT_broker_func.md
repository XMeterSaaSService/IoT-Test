开源MQTT Broker对比（ActiveMQ，EQM，Mosquitto）

|         | ActiveMQ    |  EQM  |  Mosquitto  |
| :------- | :-----:   | :----: | :----: |
| License      |  开源     |  开源版+商业版 |
| 公司／社区    |   Apache   |   EMQ   |
| 开发语言      |   java    |   Erlang    |
| 集群架构      |  支持     |   支持    |
| 系统部署      | 物理机、虚拟机、容器      |    物理机、虚拟机、容器     |
| 支持协议      | Openwire、Stomp、AMQP、MQTT、WebSocket |     MQTT、CoAP、MQTT-SN、WebSocket、JT/T808、Modbus、TCP、UDP   |
| 系统性能      |  十万级并发 |千万级并发
| MQTT版本支持  |  V3.1     | V3.1,V3.1.1,V5.0 draft|
| 管理界面界    |       |       |
| 安全与认证    | LDAP、Apache Shiro | TSL/DTLS、X.509证书、JWT、OAuth2.0、应用协议（ID/用户名密码）、认证接口（LDAP、DB、HTTP）      |
| 扩展方式      |       |  Lua hooks,Web hooks,Triggers |
| 数据存储      |JDBC、journal、KahaDB、LevelDB      | Redis、MySQL、PostgreSQL、MongoDB、LevelDB、Cassandra      |
| 数据桥接      |       | 桥接转发企业MQ:kakfa、RabbitMQ     |
| 适用场景      |  核心是企业消息队列系统，叠加支持了部分物联网协议，适合作为小型物联网系统的接入层，以及作为高吞吐量的企业消息队列     |   面向物联网特性设计，优势在于高并发连接与高吞吐消息的服务能力，以及物联网协议栈的完整性，因此更适合作为大规模物联网系统的接入与消息路由层，并可作为消息提供方挂载高吞吐的消息队列    |


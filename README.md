# meshIQa

meshIQa is messaging broker powered by [Apache ActiveMQ](https://activemq.apache.org).

It's enterprise ready messaging platform, supporting several messaging protocols:
- JMS 1.1, 2.0, 3.0
- AMQP
- MQTT
- HTTP

This distribution provides unique features on top of ActiveMQ.

## Security

meshIQa is using OAuth2 as default authentication/authorization mechanism, being able to plug with any kind of identity provider (Keycloack, ...).

Other backends are also supported (simple embedded authentication/authorization, LDAP, ...).

## Cloud

meshIQa provides the infrastructure to easily deploy on your Kubernetes environment. It includes HELM charts and unique components for replication and scalability.

## Management & Observability

meshIQa provides provides:
* console to observe and manage the destinations and broker
* Promotheus exporter

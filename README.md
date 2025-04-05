# meshIQa

```

                        __    ________        
   ____ ___  ___  _____/ /_  /  _/ __ \____ _
  / __ __  \/ _ \/ ___/ __ \ / // / / / __  /
 / / / / / /  __(__  ) / / // // /_/ / /_/ / 
/_/ /_/ /_/\___/____/_/ /_/___/\___\_\__,_/  

```

meshIQa is messaging broker powered by [Apache ActiveMQ](https://activemq.apache.org).

## Features

meshIQa is enterprise ready messaging platform, supporting several messaging protocols:
- JMS 1.1, 2.0, 3.1
- AMQP
- MQTT
- HTTP

This distribution provides unique features on top of ActiveMQ.

### Security

meshIQa is using OAuth2 as default authentication/authorization mechanism, being able to plug with any kind of identity provider (Keycloack, ...).

Other backends are also supported (simple embedded authentication/authorization, LDAP, ...).

### Cloud

meshIQa provides the infrastructure to easily deploy on your Kubernetes environment. It includes HELM charts and unique components for replication and scalability.

### Management & Observability

meshIQa provides provides:
* console to observe and manage the destinations and broker
* Promotheus exporter

## Start meshIQa

You can start meshIQa in foreground with console output:

```
$ bin/meshIQa console
INFO: Loading 'bin/setenv'
INFO: Using java '/bin/java'

                        __    ________        
   ____ ___  ___  _____/ /_  /  _/ __ \____ _
  / __ __  \/ _ \/ ___/ __ \ / // / / / __  /
 / / / / / /  __(__  ) / / // // /_/ / /_/ / 
/_/ /_/ /_/\___/____/_/ /_/___/\___\_\__,_/  

INFO: Starting in foreground, this is just for debugging purposes (stop process by pressing CTRL+C)
```

You can start meshIQa in background:

```
$ bin/meshIQa start
INFO: Loading 'bin/setenv'
INFO: Using java 'bin/java'

                        __    ________        
   ____ ___  ___  _____/ /_  /  _/ __ \____ _
  / __ __  \/ _ \/ ___/ __ \ / // / / / __  /
 / / / / / /  __(__  ) / / // // /_/ / /_/ / 
/_/ /_/ /_/\___/____/_/ /_/___/\___\_\__,_/  

INFO: Starting - inspect logfiles specified in logging.properties and log4j2.properties to get details
INFO: pidfile created : 'data/meshIQa.pid' (pid '14064')
```

Then, you can stop meshIQa with:

```
$ bin/meshIQa stop
```
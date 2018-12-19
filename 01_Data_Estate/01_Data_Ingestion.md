# Data Ingestion
This layer is primarily concerned with how we deploy, secure and update the services which are responsible for receiving massive data coming into our organization.  The Data coming could be coming from other applications (Web, API, RPC, etc), logging/telementry data (System Stats, IoT data:Sensors, etc.) or other sources like general file uploads (Word Docs, Text Files, Spreadsheets, PDFs, Images etc. etc.).

We will need to consider the type of data, the structure (if any) of the data and if it needs to be immediately accessible (searchable/queryable/readable).  This will help us determine the types of services/tools that are available to us (if any) and what our starting point will be.  We will be able to understand what the security model will look like at this level as the data could be coming in from devices, people (users) or other systems. Do we need to provision per device credentials? Are we leveraging an internal or external Authentication Service (i.e. LDAP, OAUTH etc) for users? Are other systems internally deployed or externally deployed and require implicit or explicit sources of trust?  These pieces are important at each level and will change at each respective stage.  For example Raw Storage -> Raw Data Processing is more likley an implicit trust but it can also be based on a single shared authentication token between services.

## Potential Services
### Open Source (Non-Exhaustive)
- Kafka
- Redis
- RabbitMQ
- ZeroMQ

### Azure Services
- Azure Event Hubs (Kafka Compatible API)
- Azure IoT Hub (AMQP, HTTPS, MQTT Compatible API)
- Azure Redis Cache (Redis API)
- Azure Cosmos DB (MongoDB, Cassandra and Gremlin Compatible APIs)
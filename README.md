# microservice-homework

| Products	|Kong	|Tyk	|KrakenD	|Apigee	|AWS Gateway	|Azure Gateway	|Express Gateway
|-----------|-----|-----|---------|-------|------------|--------------|--------------------
| Deployment Complexity	|Single node	|Single node	|Low, single binary	|Many nodes with different roles	|Cloud vendor PaaS	|Cloud vendor PaaS	|Flexible
| Data Stores |Required	Cassandra or Postgres	|Redis	|None	|Cassandra, Zookeeper, and Postgres	|Cloud vendor PaaS	|Cloud vendor PaaS	|Redis
| Open Source	|Yes, Apache 2.0	|Yes, MPL	|Yes, Apache 2.0	|No	|No	|No	|Yes, Apache 2.0
| Core Technology	|NGINX/Lua	|GoLang	|GoLang	|Java	|Not open	|Not open	|Node.js Express
| On Premise	|Yes	|Yes	|Yes	|Yes	|No	|No	|Yes
| Community/Extensions	|Large	|Medium	|Medium	|No	|No	|No	|Small
| Authorization/API Keys	|Yes	|Yes	|Yes	|Yes	|Yes	|Yes	|Yes
| Rate Limiting	|Yes	|Yes	|Yes	|Yes	|Yes	|Yes	|Yes
| Data Transformation	|HTTP	|HTTP	|Extensive, customizable	|Yes	|No	|No	|No
| Integrated Billing	|No	|No	|No	|Yes	|No	|No	|No

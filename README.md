# microservice-homework

### 1. Сравнительная таблица програмных предложений API-GATEWAY

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

Обоснование:

   Так как предполагается что выбор нужно сделать для крупной компании, то можем условиться, что в этом случае у нас имеется продукт обрабатывающий большой поток запросов, а также есть отдел с разработчиками.

   Для сравнения возьмем ряд самых распространеных продуктов: Kong, Tyk, KrakenD, Apigee, Aws Gateway, Azure Gateway Express Gateway.

   В списке есть облачные решения, в нашем случае можно их не рассматривать, по причине того, что облачное решение может вносить некие задержки в ответы на запросы(например на сетевом уровне), для нас это критично, а так же может произойти деградация сервиса по причинам сбоя у поставщика услуги api-gateway/

   Так как мы ищем высокпроизволительное решение, то из оставшихся самый подходящий продукт - KrakenD. KrakenD может похвастаться впечатляющими показателями производительности, способными обрабатывать более 70 000 запросов в секунду на стандартном оборудовании, что подчеркивает его эффективность и масштабируемость. 

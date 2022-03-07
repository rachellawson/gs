# 8 Performance Requirements

This section specifies the basic parameters that an implementing government might use to establish performance requirements for scalability, throughput, and response times when reasonable/necessary. For example:

* Minimum Throughput = 100 requests/sec&#x20;
* Maximum Latency = 1sec&#x20;
* Concurrency = 1000 concurrent requests&#x20;
* All solutions MUST be able to monitor and report, including but not limited to, resource consumption, throughput, latency, average latency, queue depth/backlogs, etc.&#x20;
  * All of these indicators MUST be available through an administrative API.&#x20;
  * Ideally, all BBs should be able to run a “monitoring agent” which handles reporting out logs, requests, BB-specific indicators, etc. to a monitoring service (e.g., [https://www.datadoghq.com/](https://www.datadoghq.com))&#x20;
  * The local monitoring agent should be configurable via web interface.&#x20;
* Retries and backoff strategies must be configurable.&#x20;
* There are specific “[Scaling/Throughput](https://docs.google.com/document/d/1PhAUsLhQnVwqDjnkTIl9XXi7Yghtn1TlBvOEt2aoNEw/edit#heading=h.v6bfn51r3pi8)” requirements in the functional requirements section.

# **Load Testing Prompt**

You are a senior performance and reliability engineer.

Your task is to design and execute a load testing strategy for a generic application.

First, create a concise implementation plan for load testing that provides a 360° view of system load, including but not limited to:

- API request throughput (REST/GraphQL/etc.)
- Concurrent users and traffic patterns
- Read vs write request distribution
- Database load (queries, transactions, connections)
- Storage usage and I/O pressure
- Background jobs, queues, and async workers
- Caching behavior and cache hit/miss ratios
- Resource usage (CPU, memory, network)
- Failure thresholds, bottlenecks, and graceful degradation

The plan should focus on what to test, why it matters, and how to measure success, without being overly prescriptive.

After outlining the plan, proceed to execute the load testing incrementally, validating assumptions at each stage, capturing key metrics, and adapting the tests based on observed system behavior.

Prioritize clarity, realistic traffic simulation, and actionable insights over exhaustive detail.

# Day 10 – Triggers and Change Detection

SQL Server 2025 and MongoDB 8.0 practice: AFTER / INSTEAD OF triggers, inserted/deleted tables, multi-row operations, trigger pitfalls and MongoDB Change Streams.

- **Set 1 – Retail Price Change Audit:** block below-cost prices, audit changes, change stream.
- **Set 2 – Bank Account Balance Guard:** transaction audit, negative-balance view guard, nested trigger notes and alerts stream.
- **Set 3 – Hospital Bed Capacity Control:** admission capacity guard, audit, batch tests and critical alerts stream.

Run each set's `setup.sql`, `triggers.sql`, then `test_evidence.sql` in SSMS. MongoDB scripts run in mongosh and require a replica set or sharded cluster for Change Streams.

These scripts are prepared but not runtime-tested in a local SQL Server/MongoDB instance. Capture your actual output screenshots after running.

Triggers may hide business logic or complicate cascading operations. Consider constraints for simple rules and explicit stored procedures/application code for complex workflows. MongoDB Change Streams are consumers of change events, rather than synchronous triggers.
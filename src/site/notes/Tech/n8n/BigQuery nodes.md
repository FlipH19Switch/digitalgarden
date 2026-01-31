---
{"dg-publish":true,"permalink":"/tech/n8n/big-query-nodes/","created":"2025-06-14T23:55:14.905-04:00","updated":"2025-06-14T23:55:14.905-04:00"}
---

- Execute a SQL query
	- Bulk-deleting rows >20 at a time will cause an issue
		- Add a loop before the node to loop over the individual rows to delete
		- Add a wait node with a 1-second wait after the BigQuery node to give it time to finish each query (may not be necessary)
		- Connect the wait node to the loop
		- Turn on the "Always Output Data" switch in the BigQuery node to ensure it outputs data to the wait node
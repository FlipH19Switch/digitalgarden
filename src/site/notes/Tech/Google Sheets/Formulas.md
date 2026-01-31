---
{"dg-publish":true,"permalink":"/tech/google-sheets/formulas/","created":"2025-06-14T23:55:14.904-04:00","updated":"2025-06-14T23:55:14.904-04:00"}
---

- Find duplicate values in a column:
	- =FILTER(D:D, COUNTIF(D:D, D:D) > 1)
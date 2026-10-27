---
'graphql-shield': patch
---

Generate middleware in linear time. Building the type and field maps no longer copies the accumulator for every entry, which made `shield().generate(schema)` quadratic in schema size.

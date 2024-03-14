Postgres is fully ACID compliant, meaning that it supports atomicity, consistency, isolation, and durability.

- Atomicitiy means that each command is processed as a single instruction not matter how complex it might be.
- Consistency means that the data stored in the database will be consistent throughout operations and if a operation fails the data won't be changed.
- Isolation means that the database is able to handle concurrent operations without damaging or changing the data.
- Durability means that Postgres tries to protect the data as much as it can in case of a hardware or software failure.
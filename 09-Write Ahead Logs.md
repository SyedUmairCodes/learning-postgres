Write Ahead Logs or `WALs` for short are a technology that many database systems use for their internal logging. The main concept of a `WAL` is that before confirming any operation it writes the intent as a log.

In case the cluster crashes, the database already knows what operations were completed and what data needs to be recovered when it reads the `WALs`.


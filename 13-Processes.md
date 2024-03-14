The `POSTMASTER` process is the first process that is launched when the cluster is started that is responsible for starting and managing other processes.

| Process                      | Description                                                              |
| ---------------------------- | ------------------------------------------------------------------------ |
| Checkpoint                   | Responsible for executing checkpoints that maintain the persistent data. |
| background writer            | Stores data into permanent storage from memory                           |
| walwriter                    | Writes WALs                                                              |
| logical replication launcher | Handles logical replication                                              |
> Processes are based on the configurations of the server, and so each server can have different processes running.


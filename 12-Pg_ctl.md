`Pg_ctl` is a command line utility that gets installed on your system alongside PostgreSQL and is used to manage the cluster. 

Some of the common commands are:

| Command                  | Description                                                                                                                                   |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Start, stop, and restart | Start, stops, or restarts the cluster.                                                                                                        |
| Status                   | displays the current status of the cluster.                                                                                                   |
| Init                     | Initializes a new cluster or re-initializes an already existing one. Re-initializing a cluster removes all of the previous data stored in it. |
| Reload                   | Reloads the server when there's a config change.                                                                                              |
| Promote                  | Changes a replica server to a standby one.                                                                                                    |

> Pg_ctl works with the postmaster by giving it commands that further gives commands to other services and processes. 

Pg_ctl also needs to know about the `PGDATA` directory. You can set the location of it by defining a environment variable or using the -D flag on the command line.

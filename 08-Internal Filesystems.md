In order to make the data persistent, PostgreSQL relies on the filesystem of the server it is hosted on and therefore the filesystem of the instance plays an important part in the performance of your PostgreSQL instance.

All of the internal and user data is stored in a filesystem directory called `PGDATA`. This directory represents the contents that the cluster is showing as databases. A single instance of PostgreSQL can access different `PGDATA` directories and therefore contain different databases in it.

> The PGDATA directory and it's sub-directories need to be initialized before they can be used.

The PGDATA directory is where PostgreSQL looks for its configuration and data files and also contains the `Write-Ahead-Logs` and the data storage as well.

> Without the WALs and data storage the cluster can not guarantee the consistency of the data or sometimes even start at all.

PostgreSQL runs as a service/daemon on the server or computer that it's installed on and then server is known as a cluster since it can host multiple databases.

Each database is stored in an isolated space and a user can only access a single database at a time. Users are defined cluster-wide and are not tied to a single database and can connect to as many databases as they are allowed to.

Normal users are users that are allowed to run a specific set of commands on the databases they are allowed to access. Superusers can do anything they desire with the database.

PostgreSQL stores it's internal and user data into the server's local storage in the form of catalogs that are special tables that show the specification of the instance depending on the user accessing them.
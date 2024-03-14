When the cluster is started, a single process known as the _postmaster_ is launched that bootstraps the entire instance and starts the needed processes needed to manage the database and wait for any incoming connections.

If a user connection is made over TCP/IP then the postmaster needs to fork a process called the _backend_ process that is responsible for making sure that a single user connects to the database.

> A backend process is launched for each individual connected user.




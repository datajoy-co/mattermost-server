# Getting Started

Follow [this guide](https://developers.mattermost.com/contribute/server/developer-setup/)

# Important Commands

```
make run-server
make stop-server
make stop-docker
```

The stop-server make target does not stop all the docker containers started by run-server. To stop the running docker containers:
`make stop-docker`

# Database

To interact with the database via command line use `psql --host=localhost --dbname=mattermost_test --username=mmuser` or `yarn db`.
The password is `mostest`

# Troubleshooting

If you see this error when attempting to start the server

```
ERROR: for f6221c2d95da_mattermost-postgres  Cannot start service postgres: Ports are not available: listen tcp 0.0.0.0:5432: bind: address already in use
```

Open up activity monitor, search for postgres, and stop all of the processes called postgres.

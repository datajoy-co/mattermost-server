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

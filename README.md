# esrcpg
PostgreSQL event store for the esrc project

## Features
- Implements EventStore.
- Implements EventStoreOutbox to relay events.
- Tested only for aggregate's IDs of type UUID.



## Development

[create_tables.sql](./sql/create_tables.sql) script can be used to set up your tables.

To test:
```
docker-compose up -d
go test ./...
docker-compose down --volumes
```
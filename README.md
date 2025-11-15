# MySQL BinLog

## Overview

MySQL BinLog is a MySQL Binary Log analysis tool focused exclusively on
MySQL, MariaDB, and Percona Server for MySQL, providing SQL
recovery, rollback generation, and transaction analysis capabilities
for database operations.

## Roadmap

We follow MySQL’s official release roadmap. Whenever MySQL publishes a new
major version, this project upgrades as quickly as possible to support it—
for example, we target MySQL 8.4.x today and will move to MySQL 9.7.x as soon
as it becomes available.

## Community

- Join our Telegram group to discuss SQL Labs projects, ask questions, and share feedback: https://t.me/sqllabs
- Subscribe to the Telegram channel for broadcast announcements and release news: https://t.me/sqllabschannel

## Environment

- Go 1.25.4
- MySQL 8.4.x LTS
- Ubuntu 24.04.x LTS

## Quick Start

```bash
go clean -cache -modcache -testcache -fuzzcache && rm -rf $(go env GOCACHE) $(go env GOMODCACHE)
GOOS=linux GOARCH=amd64 go build -ldflags="-s -w" -trimpath -o mysqlbinlog . && ./mysqlbinlog
```

## License

[MIT License](LICENSE)

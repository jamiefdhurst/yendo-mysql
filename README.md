# Yendo

![License](https://img.shields.io/github/license/jamiefdhurst/yendo.svg)
[![Build Status](https://ci.jamiehurst.co.uk/buildStatus/icon?job=yendo%2Fmaster)](https://ci.jamiehurst.co.uk/job/yendo/job/master/)
[![Latest Version](https://img.shields.io/github/release/jamiefdhurst/yendo.svg)](https://github.com/jamiefdhurst/yendo/releases)

A small and simple MySQL database package for Go that includes support for automatic migrations.

## Usage Example

A detailed example is present in the `example/` folder. 

## Running Tests

The tests require a MySQL connection available - the following environment variables are used to establish the 
connection:

* `DB_HOST` - Hostname or IP address, e.g. `localhost`
* `DB_PORT` - Port number, usually 3306 - this can be ommitted
* `DB_USER` - Username to connect as
* `DB_PASSWORD` - Password to connect using
* `DB_NAME` - Database name to use when testing

You can optionally pass a `DB_MIGRATION_FOLDER` environment variable to point to the current root of the package, so
the tests can make use of the test migration data.

Once these conditions are met, the tests can be performed simply by running:

```bash
go test -v
```
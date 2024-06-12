

# Hashgrits - an implementation of the REDIS server protocol with direct integration into a PostgreSQL instance
via an extension.

## Features

* Basic Redis server command support (get/put) into a postgres backed table.
* Basic Redis operations for data structures (list like BLMOVE, BLPOP, etc)  full list tbd.
* Table mapping into redis space, so that a table or view can be mapped into the redis keyspace and accessed via Redis protocol.

## Projects

* Phase 1
** Setup build system for zig code
** Create basic zig framework and skeleton for server
** Setup unit testing framework for server
** Setup zig server for listening for commands
** Implement simple hash table for redis backing before postgres integration.
** Test cases by manually sending commands
* Phase 2
** Implement basic Redis parser for server
* Phase 3
** Figure out how to build zig extension for postgres
* Postgres hermetic environment in docker for testing.


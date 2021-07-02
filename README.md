# Flink Cassandra connector unbundled
[![CI Status](https://github.com/findify/flink-connector-cassandra/workflows/maven/badge.svg)](https://github.com/findify/flink-connector-cassandra/actions)
[![License: Apache 2](https://img.shields.io/badge/License-Apache2-green.svg)](https://opensource.org/licenses/Apache-2.0)
![Last commit](https://img.shields.io/github/last-commit/findify/flink-connector-cassandra)
![Last release](https://img.shields.io/github/release/findify/flink-connector-cassandra)

This project is a forked version of an official Flink Cassandra connector, but
with the following changes:
* Cassandra driver is upgraded to the latest 3.10 version (instead of 5 year old 3.0)
* Driver code is not bundled into the jar, so there won't be classpath conflicts
on building fat jars
* Migrated to the more recent Guava 27.x so it won't conflict with the Flink's one.

## Usage

To install, use the following maven coordinates:
```xml
<dependency>
  <groupId>io.findify</groupId>
  <artifactId>flink-connector-cassandra_2.12</artifactId>
  <version>1.13.1-1</version>
</dependency>
```

Versioning schema attempts to match the upstream, but with extra -N suffix, if there were a couple of extra code 
changes released on top.

## License

Featury is licensed under the Apache 2.0.
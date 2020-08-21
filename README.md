[![Build Status](https://travis-ci.org/avro-kotlin/avro4k-arrow.svg?branch=master)](https://travis-ci.org/avro-kotlin/avro4k-arrow)
[<img src="https://img.shields.io/maven-central/v/com.sksamuel.avro4k/avro4k-arrow.svg?label=latest%20release"/>](http://search.maven.org/#search%7Cga%7C1%7Cavro4k)
[<img src="https://img.shields.io/nexus/s/https/oss.sonatype.org/com.sksamuel.avro4k/avro4k-arrow.svg?label=latest%20snapshot&style=plastic"/>](https://oss.sonatype.org/content/repositories/snapshots/com/sksamuel/avro4k/avro4k-arrow/)


## Introduction

Avro4k-Arrow is a library that provides avro4k serializers for arrow types.

This library provides serializers for the following arrow types:

| JVM Type                   	| Schema Type   	| Logical Type     	| Encoded Type |
|------------------------------	|---------------	|------------------	| ------------ |
| arrow.core.Option<T>          | UNION<null, T>    |                   | null, T |
| arrow.core.Tuple2<A,B>        | RECORD<A,B>       |                   | GenericRecord |
| arrow.core.Tuple3<A,B,C>      | RECORD<A,B,C>     |                   | GenericRecord |


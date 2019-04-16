Agrona
======

[![Javadocs](http://www.javadoc.io/badge/org.agrona/agrona.svg)](http://www.javadoc.io/doc/org.agrona/agrona)

Agrona provides a library of data structures and utility methods that are a common need when building high-performance 
applications in Java. Many of these utilities are used in the [Aeron](https://github.com/real-logic/aeron) 
efficient reliable UDP unicast, multicast, and IPC message transport and provides high-performance buffer implementations
to support the [Simple Binary Encoding](https://github.com/real-logic/simple-binary-encoding) Message Codec.

For the latest version information and changes see the [Change Log](https://github.com/real-logic/agrona/wiki/Change-Log). 

The latest release and **downloads** can be found in [Maven Central](http://search.maven.org/#search%7Cga%7C1%7Cagrona).

Utilities Included:

* Buffers - Thread safe direct and atomic for working with on and off heap memory with memory ordering semantics.
* Lists - Array backed lists of int/long primitives to avoid boxing.
* Maps - Open addressing and linear probing with int/long primitive keys to object reference values.
* Maps - Open addressing and linear probing with int/long primitive keys to int/long values.
* Sets - Open addressing and linear probing for int/long primitives and object references.
* Cache - Set Associative with int/long primitive keys to object reference values.
* Clocks - Clock implementations to abstract system clocks, allow caching, and enable testing.
* Queues - Lock-less implementations for low-latency applications.
* Ring/Broadcast Buffers - implemented off-heap for IPC communication.
* Basic Agent framework.
* Signal handling to support "Ctrl + c" in a server application.
* Scalable Timer Wheel.
* Basic code generation from annotated implementations that can vary on primitive types.
* Off-heap counters implementation for application telemetry and position tracking.
* Implementations of InputStream and OutputStream that can wrap direct buffers.
* DistinctErrorLog: A log of distinct errors to avoid filling disks with existing logging approaches.

Build
-----

### Java Build

The project is built with [Gradle](http://gradle.org/) using this [build.gradle](https://github.com/real-logic/agrona/blob/master/build.gradle) file.

You require the following to build Agrona:

* Latest stable [Oracle JDK 8](http://www.oracle.com/technetwork/java/)

Full clean, build, and install into local maven repository

    $ ./gradlew

License (See LICENSE file for full license)
-------------------------------------------
Copyright 2014-2018 Real Logic Limited

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

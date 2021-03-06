# Play Framework Integration <img align="right" src="https://rawgit.com/kamon-io/Kamon/master/kamon-logo.svg" height="150px" style="padding-left: 20px"/>
![Build Status](https://travis-ci.org/kamon-io/kamon-play.svg?branch=kamon-1.0)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/kamon-io/Kamon?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[ ![Download](https://api.bintray.com/packages/kamon-io/snapshots/kamon-play/images/download.svg) ](https://bintray.com/kamon-io/snapshots/kamon-play/_latestVersion)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.kamon/kamon-play-2.6_2.12/badge.svg)](https://maven-badges.herokuapp.com/maven-central/io.kamon/kamon-play-2.6_2.12)

The `kamon-play` module ships with bytecode instrumentation that brings automatic traces and spans management to your Play! applications. The details on what those features are about can be found
in the [base functionality] documentation section. Here we will dig into the specific aspects of bringing support for them when using
Play!.

The <b>kamon-play</b> module requires you to start your application using the AspectJ Weaver Agent. Kamon will warn you
at startup if you failed to do so.

Since Kamon 1.0.0 we support Play Framework 2.4, 2.5 and 2.6!. Please make sure you add either <b>kamon-play-24</b>, <b>kamon-play-25</b> or <b>kamon-play-26</b> to your project's classpath.

### Getting Started

Kamon Play is currently available for Scala 2.10, 2.11 and 2.12.

Supported releases and dependencies are shown below.

| kamon-play-2.4  | status | jdk  | scala            
|:------:|:------:|:----:|------------------
|  1.0.1 | stable | 1.7+, 1.8+ | 2.10, 2.11

| kamon-play-2.5  | status | jdk  | scala   
|:------:|:------:|:----:|------------------
|  1.0.1 | stable | 1.7+, 1.8+ | 2.11

| kamon-play-2.6  | status | jdk  | scala   
|:------:|:------:|:----:|------------------
|  1.0.1 | stable | 1.8+ | 2.12  


To get started with SBT, simply add the following to your `build.sbt` or `pom.xml`
file:

```scala
libraryDependencies += "io.kamon" %% "kamon-play-[play-version]" % "1.0.1"
```

```xml
<dependency>
    <groupId>io.kamon</groupId>
    <artifactId>kamon-play-[play-version]_2.12</artifactId>
    <version>1.0.1</version>
</dependency>
```
[base functionality]: http://kamon.io/integrations/web-and-http-toolkits/base-functionality/

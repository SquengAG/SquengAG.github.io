---
layout: default
title: Squeng AG
description: building the right thing right
---

{% include navigation.md %}

## Spring

### Create Project

There are various ways to create a Spring Boot project. My preferred way is to use the [Spring Initializr](https://start.spring.io/):

![Init](SIleft.png)

(At the time of this writing, Kotlin does not support Java 25, which is why the language version in `build.gradle.kts` would have been tacitly reduced to 24 if we had chossen Kotlin as the language.)

As for the dependencies, we can start with as little as Spring Web only, but **we must not postpone including Spring Security for too long** …

![Dependencies](SIright.png)

Note that a few versions ago, I would have included Spring Reactive Web instead of Spring Web. But now that Spring supports [Virtual Threads](https://dev.java/learn/new-features/virtual-threads/) and since [Spring's asynchronous model](https://docs.spring.io/spring-framework/reference/web-reactive.html) based on [Project Reactor](https://projectreactor.io/) was never pleasant to work with (unlike [Play's asynchronous model](https://www.playframework.com/documentation/latest/ScalaAsync) based on [Scala Futures](https://docs.scala-lang.org/overviews/core/futures.html)), I am more than happy to switch back to Spring Web, but we must remember to enable Virtual Threads in `src/main/resources/application.properties`:

```
spring.threads.virtual.enabled=true
```

### Create Subproject

In order to protect the business logic / domain from the harsh world around it (the Web framework, the DBMS, etc.), I am applying the [Ports & Adapters](https://alistaircockburn.company.site/Epub-Hexagonal-Architecture-Explained-Updated-1st-ed-p751233517) pattern. I could do so within the main project, but I prefer to take advantage of Gradle's support for [multi-project builds](https://docs.gradle.org/current/userguide/multi_project_builds.html) so that Gradle can help enforcing the boundary.

Furthermore, I want to implement the business logic / domain in Scala, which Gradle supports through its [Scala plugin](https://docs.gradle.org/current/userguide/scala_plugin.html).

Prepare the folders:

- within the project folder, alongside the existing `src` folder, create a folder `hexagon`
- within folder `hexagon`, create another `src` folder 
- within folder `hexagon/src`, create folders `main` and `test`
- within folder `hexagon/src/main`, create folders `resources` and `scala`
- within folder `hexagon/src/test`, create folder `scala`

Prepare the configuration:

- within the existing `build.gradle.kts` file, add the subproject as well as the [Scala library](https://mvnrepository.com/artifact/org.scala-lang/scala3-library) as dependencies:

```
dependencies {
    implementation(project(":hexagon"))
    implementation("org.scala-lang:scala3-library_3:3.3.7")

    implementation("org.springframework.boot:spring-boot-starter-webmvc")
```

- within the existing `settings.gradle.kts` file, add the subproject as well:

```
rootProject.name = "spring-clean"
include("hexagon")
```

- within folder `hexagon`, create another file `build.gradle.kts` with the following content:

```
plugins
{
    id("scala")
}

repositories {
    mavenCentral()
}

scala {
    scalaVersion = "3.3.7"
}
```

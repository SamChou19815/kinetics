# KineticS

[![Build Status](https://travis-ci.com/SamChou19815/kinetics.svg?branch=master)](https://travis-ci.com/SamChou19815/kinetics)
[![Release](https://jitpack.io/v/SamChou19815/kinetics.svg)](https://jitpack.io/#SamChou19815/kinetics)
![GitHub](https://img.shields.io/github/license/SamChou19815/kinetics.svg)

KineticS is an opinionated Kotlin library to quickly bootstrap your backend on Google Cloud
Platform.

Currently, the library contains the out-of-the-box implementation for:

- An account system based on Firebase.
- Authentication and authorization system based on Firebase and Spark PAC4J.
- A simple friend system with already defined database structure and easy-to-use APIs.
- Imported a type-safe client library for Google Datastore. [TypedStore](https://github.com/SamChou19815/typed-store)

The project is in beta, which means all APIs are subject to change. You should not use this for very
serious stuff (e.g. serving millions of users), but you can freely use it during Hackathon (that's
exactly what this library is designed for).

## Gradle Config

Add this to your `build.gradle` to use the artifact.

```groovy
repositories {
    jcenter()
    maven { url "https://jitpack.io" }
}
dependencies {
    implementation 'com.github.SamChou19815:kinetics:+'
}
```

## Config Files

The library uses Google's default credential. You need to property setup your GCP credential in
your development environment.

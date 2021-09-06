---
description: >-
  A Kotlin-based HTML / XML deserialization library that places particular
  emphasis on ease of use and a high level of readability by providing an
  intuitive DSL.
---

# Introduction

{% hint style="info" %}
[**skrape{it}**](http://www.skrape.it) is a Kotlin-based HTML/XML testing and web scraping library that can be used seamlessly in Spring-Boot, Ktor, Android or other Kotlin-JVM projects. The ability to **analyze and extract HTML including client-side rendered DOM trees** and all other XML-related markup specifications such as SVG, UML, RSS,... makes it unique. It places particular emphasis on **ease of use** and a **high level of readability** by providing an **intuitive DSL**. First and foremost skrape{it} aims to be a testing tool \(not tied to a particular test runner\), but it can also be used to scrape websites in a convenient fashion.
{% endhint %}

### Focus and Paradigms

#### Idomatic

* [x] Easy to use, idiomatic and type-safe DSL to ensure a high level of readability.
* [x] DSL is behaving like a Fluent-Api to make data extraction/scraping as comfortable as possible.

#### Compatibility

* [x] Not bind to a specific test-runner, framework or whatever.
* [x] Open to easily use it with any of your favorite assertion or http client library.
* [x] Open to implement your own fetcher
* [x] Supports non-blocking fetching / Coroutine support
* [x] Extensions for other well-known libraries

### Features

**The library provides 3 main features.**   
All the features can be used together. This will give you super smooth and highly readable user experience. But it is perfectly fine and possible to use only individual aspects. 

#### Parsing

* [x] Deserialization of HTML/XML from websites, local html files and html as string to data classes / POJOs.
* [x] Designed to deserialize HTML but can handle any XML-related markup specifications such as SVG, UML, RSS or XML itself.
* [x] DSL to select html elements as well as supporting CSS query-selector syntax by string invocation.
* [x] Support to parse HTML after javascript execution.

#### Http-Client

* [x] Http-Client without verbosity and ceremony to make requests and corresponding request options like headers, cookies etc in a fluent style interface.
* [x] Pre-configure client regarding auth and other request settings
* [x] Can handle client side rendered web pages. Javascript execution results can optionally be considered in the response body.

**Assertions**

* [x] Build-in HMTL document specific matchers 
* [x] Build-in matchers/assertions based on infix functions to archive a very high level of readability.
* [x] open to use your own matchers

{% hint style="info" %}
The skrape{it} library is a multi-module project where basically every module is responsible for one feature.  
So if you for example just want to parse HTML from String and have to take care about the size of you dependency-tree it is possible to just add single features as a dependency to your project.
{% endhint %}


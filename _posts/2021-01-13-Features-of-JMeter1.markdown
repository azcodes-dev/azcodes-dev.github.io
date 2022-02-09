---
layout: post
title:  Features of JMeter and Visual Studio
description: Similar terminologies of VS Load Test Framework present in JMeter
date:   2021-01-13 20:00:00 +0400
image:  '/images/jmeter.jpg'
tags:   [performanceengineering]
featured: true
---
Microsoft had announced during the release of Microsoft Visual Studio 2019 that the Web Performance and Load Test feature is being deprecated and Visual Studio 2019 will be the last one having this feature. For more info, read directly from this [Microsoft Blog](https://devblogs.microsoft.com/devops/cloud-based-load-testing-service-eol/). This announcement had triggered several questions being asked by performance/test engineers and developers who have been using Visual Studio to carry out web performance test development and load testing for years. The most asked question has been  

> Which tool should we migrate to?

There are several tools in the market like Apache JMeter, K6, Gatling, Neoload, Blazemeter, Load Runner, and so on.
However, the most used and having the largest community is the open-sourced Apache JMeter, which is one of the recommended tool by Microsoft.

Here are some of the concept/terminology of Visual Studio and the equivalent of Apache JMeter.

Visual Studio | JMeter
------------- | -------
Web request  | Sampler -> HTTP request
Headers of web request | Config -> HTTP Header Manager
Validation rules | Assertions
Extraction rules | Post processors
Conditions/Decisions/Loops | Logic controllers -> If, Loop and While controllers
Transactions | Logic controllers -> Transaction controllers
Web test | Test fragment
Call to web test | Logic controllers -> Module controllers
Context parameters | User defined Variables
Data sources | Config element -> CSV Data Set Config or JDBC request
Virtual users, Load patterns and duration | Thread Groups setting
Credentials | Config Element -> HTTP Authorization Manager
Web test plugins | JSR223 Sampler
Request plugins | JSR223 Pre/Post processors

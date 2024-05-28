# function-performance-logger
A lightweight utility for logging and analyzing function performance in JavaScript applications.

## Overview
PerformanceLogger is a class designed to provide insight into the performance of JavaScript functions. By logging the start and end times of function executions, as well as optional stack traces, it allows developers to identify potential bottlenecks and optimize code for improved efficiency.

## Features
### Function Performance Tracking 
Monitor the execution time of specific functions within your codebase.
### Stack Trace Collection 
Optionally collect stack traces to gain deeper insights into function calls and their context.
### Flexible Integration 
Easily integrate PerformanceLogger into your existing codebase with minimal setup required.
### Node.js Support 
Compatible with both browser-based and Node.js environments.

## Usage web

```javascript
  PerformanceLogger.watch({name of Object}, "{function Name as string}", true);
  // e.g. PerformanceLogger.watch(window, "someFunc", true);
  console.log(PerformanceLogger.watchedFunctionsStats);
  console.log(PerformanceLogger.watchedFunctionsMessages);
```

## Usage nodejs 

install with:
```sh
npm i function-performance-logger
```

```javascript
  // You need global PerformanceLogger object written exactly as PerformanceLogger
  PerformanceLogger = require('function-performance-logger');
  PerformanceLogger.watch({name of Object}, "{function Name as string}", true);
  // e.g. PerformanceLogger.watch(window, "someFunc", true);
  console.log(PerformanceLogger.watchedFunctionsStats);
  console.log(PerformanceLogger.watchedFunctionsMessages);
```

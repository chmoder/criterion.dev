# criterion.dev
The official support channel for [https://api.criterion.dev](https://api.criterion.dev) and [https://criterion.dev](https://criterion.dev)

### About
Criterion.dev is a service for tracking the performance of an application.  The inspiration for this service comes from classic technical debt scenarios where as a project is enhanced over time and performance regresses simply because it is not being monitored.

Criterion.dev aims to provide a service that developers can add to their CI/CD flows to proactively track the performance of software at the method level using benchmark frameworks.  The first framework supported at criterion.dev will be the [criterion-rs](https://github.com/bheisler/criterion.rs) benchmark framework.  

### Goals
1) Code coverage
2) Documentation
3) Automate builds, and deployment to k8 or something
4) Add JWT support
5) User interfaces for viewing uploaded reports with #commit
6) More frameworks
7) Github, bitbucket, and gitlab integration
8) The sky's the limit

### Usage
Start by following [this guide](https://bheisler.github.io/criterion.rs/book/getting_started.html), to set up your project with benchmarks
In your projects root directory, these commands will run the benchmarks, and upload the measurements to crition.dev.

`cargo bench -- --verbose --noplot`
```
export CRITERION_TOKEN="token"
bash <(curl -s https://criterion.dev/bash)
```

### Issues and Feature Requests
If you have a bug to report, or a feature request, please open an issue here.  We love to get feedback, suggestions, and even new contributors.  

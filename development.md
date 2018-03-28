# Building high quality service APIs
* Within major versions, services are backwards compatible
* Backwards compatibility -> client does not need to change
* Only two good ways to implement 99% of typical web services now
  * Clusters for containers (Kubernetes/Docker) with [12-factor](https://12factor.net/) patterns
  * Function-as-a-Service (Lambda, Azure)

# Languages and productivity
* Statically-typed, fast-by-default languages generally beat dynamically-typed and interpreted (provided 'Any' is available when needed)
* Key traits: conciseness, clarity, DRY, leverage across platforms, community and toolchain/IDE support
* REPL can be helpful
* At small scale, you won't notice a difference between say Javascript and Typescript. But large scale, you'll wish you had made the right choice to begin with.
* Best current languages<sup>1</sup> by purpose
  * Client Devices and/or Services: Kotlin or C#
  * Web Clients and/or Services: Typescript
  * Close to metal: C++ or Rust
  * High concurrency network services: Elixir (not personally tested)
* For the future, I think Crystal and PyPy are interesting projects. Especially Crystal, as it has some sophisticated systems-level programming constructs you can 'drop' into when necessary, but for the most part are high level. In terms of performance may be close enough to C++/Rust for most services.

<sup>1</sup>Yes, this is somewhat a jumble of language plus platform.

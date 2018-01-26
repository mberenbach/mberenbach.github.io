# Building high quality service APIs
* Within major versions, services are backwards compatible
* Backwards compatibility -> client does not need to change
* Only two good ways to implement 99% of typical web services now
  * Clusters for containers (Kubernetes/Docker) with [12-factor](https://12factor.net/) patterns
  * Function-as-a-Service (Lambda, Azure)

# Languages and productivity
* Statically-typed, fast-by-default languages generally beat dynamically-typed and interpreted (provided 'Any' is available when needed)
* Key traits: conciseness, clarity, DRY, leverage across platforms, community and toolchain/IDE support
* At small scale, you won't notice a difference between say Javascript and Typescript. At large scale, you'll wish you had made the right choice to begin with.
* Best current languages<sup>1</sup> by purpose
  * JVM/Android/Services: Kotlin
  * Web/Services: Typescript
  * Close to metal: C++ or Rust
  * High concurrency network services: Elixir (not personally tested)
* Most interesting new general purpose language: Crystal

<sup>1</sup>Yes, this is somewhat a jumble of language plus platform. However, the language is the user interface to the platform.

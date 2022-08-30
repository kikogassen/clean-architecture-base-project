# Clean Architecture - base project

This repository can be forked to be used as a base of Clean Architecture project. It has the following filetree:

```
project
├───app
│   │   build.gradle
│   │   proguard-rules.pro
│   │
│   └───src
│
├───features // all aplication features
│   └───home
│
├───foundation
│   ├───core
│   ├───core-android
│   ├───data
│   ├───domain
│   ├───dsc
│   ├───monitoring
│   └───navigation
```

## General information

- Three flavors (`dev`, `beta` and `prod`) with its respective application name and `applicationId`;
- Single activity design pattern to allow deeplinking and internal navigation;
- `:features` modules without circular dependency;
- `:foundation` modules to be used in all `:features` modules;
- Clean and lightweight `:app` module.
- For this project there is not a dependency injection library integrated since there are two common libraries for this: [Hilt](https://developer.android.com/training/dependency-injection/hilt-android) and [Koin](https://insert-koin.io/docs/quickstart/android/).
